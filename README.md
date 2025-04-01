# Manohar-Kumar-
Online gameplay 
https://www.effectiveratecpm.com/t0tie8wi?key=032c20bd6a30eb839f6e3e3480f5b38c
import { useState } from "react"; import { io } from "socket.io-client"; import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card";

const socket = io("http://localhost:4000");

export default function Game() { const [players, setPlayers] = useState([]); const [gameState, setGameState] = useState("Waiting for players...");

socket.on("updatePlayers", (playerList) => { setPlayers(playerList); });

socket.on("gameState", (state) => { setGameState(state); });

const joinGame = () => { socket.emit("joinGame", { name: "Player" + (players.length + 1) }); };

return ( <div className="p-4 flex flex-col items-center"> <h1 className="text-2xl font-bold">Online Gameplay</h1> <p className="mb-4">{gameState}</p> <Button onClick={joinGame}>Join Game</Button> <div className="mt-4 grid grid-cols-2 gap-2"> {players.map((player, index) => ( <Card key={index}> <CardContent className="p-2">{player.name}</CardContent> </Card> ))} </div> </div> ); }

