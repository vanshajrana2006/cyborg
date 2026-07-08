# cyborg
import React from "react";
import { motion } from "framer-motion";

export default function CyborgLandingPage() {
  return (
    <div className="min-h-screen bg-black text-white font-sans">
      {/* Navbar */}
      <nav className="flex justify-between items-center p-6 border-b border-gray-800">
        <h1 className="text-2xl font-bold tracking-widest text-cyan-400">CYBORG-X</h1>
        <div className="space-x-6 hidden md:flex">
          <a href="#" className="hover:text-cyan-400">Home</a>
          <a href="#" className="hover:text-cyan-400">Features</a>
          <a href="#" className="hover:text-cyan-400">Tech</a>
          <a href="#" className="hover:text-cyan-400">Contact</a>
        </div>
      </nav>

 
  );
}
