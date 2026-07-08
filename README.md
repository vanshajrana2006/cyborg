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

      {/* Hero Section */}
      <section className="flex flex-col md:flex-row items-center justify-between px-8 md:px-20 py-16">
        <motion.div
          initial={{ opacity: 0, x: -50 }}
          animate={{ opacity: 1, x: 0 }}
          transition={{ duration: 0.8 }}
          className="max-w-lg"
        >
          <h2 className="text-4xl md:text-6xl font-bold leading-tight">
            The Future is <span className="text-cyan-400">Augmented</span>
          </h2>
          <p className="mt-6 text-gray-400">
            Experience next-gen human-machine integration with cutting-edge
            cyborg enhancements designed for speed, intelligence, and power.
          </p>
          <button className="mt-8 px-6 py-3 bg-cyan-500 rounded-xl shadow-lg hover:bg-cyan-400 transition">
            Explore Now
          </button>
        </motion.div>

        <motion.div
          initial={{ opacity: 0, x: 50 }}
          animate={{ opacity: 1, x: 0 }}
          transition={{ duration: 0.8 }}
          className="mt-10 md:mt-0"
        >
          <div className="w-72 h-72 bg-gradient-to-r from-cyan-500 to-purple-600 rounded-full blur-3xl opacity-30"></div>
        </motion.div>
      </section>

      {/* Features */}
      <section className="px-8 md:px-20 py-16 grid md:grid-cols-3 gap-8">
        {["AI Integration", "Neural Boost", "Cyber Defense"].map((feature, i) => (
          <motion.div
            key={i}
            whileHover={{ scale: 1.05 }}
            className="p-6 bg-gray-900 rounded-2xl border border-gray-800 shadow-lg"
          >
            <h3 className="text-xl font-semibold text-cyan-400">{feature}</h3>
            <p className="mt-4 text-gray-400">
              Advanced {feature.toLowerCase()} technology for enhanced human
              capabilities.
            </p>
          </motion.div>
        ))}
      </section>

      {/* CTA */}
      <section className="text-center py-20 border-t border-gray-800">
        <h2 className="text-3xl md:text-5xl font-bold">
          Upgrade Your Reality
        </h2>
        <button className="mt-8 px-8 py-4 bg-purple-600 rounded-2xl hover:bg-purple-500 transition">
          Join the Revolution
        </button>
      </section>

      {/* Footer */}
      <footer className="text-center p-6 border-t border-gray-800 text-gray-500">
        © 2026 CYBORG-X. All rights reserved.
      </footer>
    </div>
  );
}
