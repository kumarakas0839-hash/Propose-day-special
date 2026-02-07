import React, { useState, useEffect } from "react";
import { motion, AnimatePresence } from "framer-motion";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

export default function ProposeDayWebsite() {
  const [stage, setStage] = useState("box");
  const [nameInput, setNameInput] = useState("");
  const [error, setError] = useState("");
  const [timeLeft, setTimeLeft] = useState("");
  const [noOffset, setNoOffset] = useState({ x: 0, y: 0 });
  const [heartRain, setHeartRain] = useState(false);
  const [sparkleRain, setSparkleRain] = useState(false);
  const [fireworks, setFireworks] = useState(false);
  const [showFavorites, setShowFavorites] = useState(false);
  const [showFairyText, setShowFairyText] = useState(false);

  const meetingDate = new Date("2026-01-22T22:30:00");

  // Countdown Timer
  useEffect(() => {
    if (stage !== "countdown") return;

    const interval = setInterval(() => {
      const now = new Date();
      const diff = now - meetingDate;

      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
      const minutes = Math.floor((diff / (1000 * 60)) % 60);
      const seconds = Math.floor((diff / 1000) % 60);

      setTimeLeft(`${days}d ${hours}h ${minutes}m ${seconds}s Together ❤️`);
    }, 1000);

    return () => clearInterval(interval);
  }, [stage]);

  // Moving NO button
  useEffect(() => {
    if (stage !== "proposal") return;

    const interval = setInterval(() => {
      setNoOffset({
        x: Math.random() * 320 - 160,
        y: Math.random() * 220 - 110,
      });
    }, 700);

    return () => clearInterval(interval);
  }, [stage]);

  const handleNameSubmit = () => {
    if (nameInput.trim().toLowerCase() === "sushma") {
      setShowFairyText(true);
      setTimeout(() => {
        setStage("countdown");
        setShowFairyText(false);
      }, 2500);
    } else {
      setError("Only Sushma can open this surprise 💖");
    }
  };

  const handleYes = () => {
    setHeartRain(true);
    setSparkleRain(true);
    setFireworks(true);

    if (navigator.vibrate) {
      navigator.vibrate([200, 100, 200, 100, 300]);
    }

    setTimeout(() => {
      setFireworks(false);
      setStage("envelope");
    }, 3000);
  };

  return (
    <div className="min-h-screen bg-gradient-to-br from-pink-100 via-rose-100 to-pink-200 flex items-center justify-center p-6 relative overflow-hidden">

      {/* Fireworks ONLY during proposal Yes moment */}
      {stage === "proposal" && fireworks && (
        <div className="absolute inset-0 pointer-events-none">
          {[...Array(25)].map((_, i) => (
            <motion.div
              key={i}
              initial={{ scale: 0, opacity: 1 }}
              animate={{ scale: 3, opacity: 0 }}
              transition={{ duration: 1.2, repeat: Infinity, delay: Math.random() }}
              className="absolute text-3xl"
              style={{
                top: Math.random() * 100 + "%",
                left: Math.random() * 100 + "%",
              }}
            >
              🎆
            </motion.div>
          ))}
        </div>
      )}

      {/* Heart Shower */}
      {heartRain && (
        <div className="absolute inset-0 pointer-events-none">
          {[...Array(30)].map((_, i) => (
            <motion.div
              key={i}
              initial={{ y: -50, x: Math.random() * window.innerWidth }}
              animate={{ y: window.innerHeight + 50 }}
              transition={{ duration: 3 + Math.random() * 2 }}
              className="absolute text-2xl"
            >
              ❤️
            </motion.div>
          ))}
        </div>
      )}

      {/* Sparkle Shower */}
      {sparkleRain && (
        <div className="absolute inset-0 pointer-events-none">
          {[...Array(35)].map((_, i) => (
            <motion.div
              key={i}
              initial={{ y: -50, x: Math.random() * window.innerWidth }}
              animate={{ y: window.innerHeight + 50 }}
              transition={{ duration: 2 + Math.random() * 2 }}
              className="absolute text-xl"
            >
              ✨
            </motion.div>
          ))}
        </div>
      )}

      <AnimatePresence>
        {/* Surprise Box */}
        {stage === "box" && (
          <motion.div initial={{ scale: 0 }} animate={{ scale: 1 }} className="text-center">
            <Card className="rounded-2xl shadow-xl">
              <CardContent className="p-10 space-y-6">
                <motion.div
                  whileHover={{ scale: 1.1 }}
                  whileTap={{ scale: 0.9 }}
                  onClick={() => {
                    setHeartRain(true);
                    setSparkleRain(true);
                    setStage("name");
                  }}
                  className="text-6xl cursor-pointer"
                >
                  🎁
                </motion.div>
                <p>Click The Surprise Box</p>
              </CardContent>
            </Card>
          </motion.div>
        )}

        {/* Name */}
        {stage === "name" && (
          <motion.div initial={{ opacity: 0 }} animate={{ opacity: 1 }}>
            <Card className="rounded-2xl shadow-xl">
              <CardContent className="p-10 space-y-6 text-center">
                <h1 className="text-2xl font-bold text-rose-600">Enter Your Name</h1>
                <input
                  value={nameInput}
                  onChange={(e) => setNameInput(e.target.value)}
                  className="border rounded-xl px-4 py-2 w-full"
                  placeholder="Enter your name"
                />
                {error && <p className="text-red-500">{error}</p>}
                <Button onClick={handleNameSubmit}>Open</Button>
              </CardContent>
            </Card>

            {showFairyText && (
              <motion.div
                initial={{ opacity: 0, y: 40 }}
                animate={{ opacity: 1, y: 0 }}
                className="mt-6 text-2xl font-bold text-rose-600"
              >
                ✨ The Fairy Has Arrived ✨
              </motion.div>
            )}
          </motion.div>
        )}

        {/* Countdown */}
        {stage === "countdown" && (
          <motion.div initial={{ opacity: 0 }} animate={{ opacity: 1 }} className="text-center space-y-6">
            <h1 className="text-4xl font-bold text-rose-600">Since We First Met ❤️</h1>
            <p className="text-2xl font-semibold">{timeLeft}</p>
            <p>22 Jan 2026 at 10:30 PM on Ome TV 💫</p>
            <Button onClick={() => setStage("proposal")}>Next</Button>
          </motion.div>
        )}

        {/* Proposal Scene */}
        {stage === "proposal" && (
          <motion.div initial={{ opacity: 0 }} animate={{ opacity: 1 }} className="text-center space-y-6">
            <motion.div
              initial={{ x: -300 }}
              animate={{ x: 0 }}
              transition={{ duration: 1.5 }}
              className="text-7xl"
            >
              🤵🌹
            </motion.div>
            <h2 className="text-3xl font-bold text-rose-600">Will You Accept My Proposal?</h2>
            <div className="flex gap-6 justify-center relative">
              <Button onClick={handleYes}>Yes ❤️</Button>
              <motion.div animate={noOffset} transition={{ type: "spring" }}>
                <Button variant="outline">No 😜</Button>
              </motion.div>
            </div>
          </motion.div>
        )}

        {/* Animated Envelope */}
        {stage === "envelope" && (
          <motion.div className="text-center space-y-6">
            <h2 className="text-3xl font-bold text-rose-600">A Surprise For You 💌</h2>
            <motion.div
              className="text-7xl cursor-pointer"
              initial={{ scale: 0 }}
              animate={{ scale: 1 }}
              whileHover={{ scale: 1.1 }}
              whileTap={{ scale: 0.9 }}
              onClick={() => setStage("special")}
            >
              💌
            </motion.div>
            <p>Click The Envelope</p>
          </motion.div>
        )}

        {/* What Makes You Special */}
        {stage === "special" && (
          <motion.div className="text-center space-y-6">
            <h2 className="text-3xl font-bold text-rose-600">What Makes You Special 💖</h2>
            <ul className="text-lg space-y-2">
              <li>✨ Your Beautiful Smile</li>
              <li>✨ Your Pure Heart & Kind Nature</li>
              <li>✨ Your Sweet Voice</li>
              <li>✨ Your Cute Expressions</li>
              <li>✨ Your Positive Energy</li>
              <li>✨ Your Simplicity</li>
              <li>✨ Your Caring Nature</li>
              <li>✨ The Happiness You Spread</li>
              <li>✨ The Way You Make People Feel Safe</li>
              <li>✨ Your Soft and Pure Soul</li>
              <li>✨ Your Honest Heart</li>
              <li>✨ Your Natural Beauty</li>
              <li>✨ Your Magical Presence</li>
            </ul>
            <Button onClick={() => setStage("favoritesGate")}>Next</Button>
          </motion.div>
        )}

        {/* Favorites Heart Gate */}
        {stage === "favoritesGate" && (
          <motion.div className="text-center space-y-6">
            <h2 className="text-2xl font-bold text-rose-600">Click Heart To See Favorites 💕</h2>
            <motion.div
              className="text-6xl cursor-pointer"
              whileTap={{ scale: 0.8 }}
              whileHover={{ scale: 1.2 }}
              onClick={() => setShowFavorites(true)}
            >
              ❤️
            </motion.div>

            {showFavorites && (
              <motion.ul initial={{ opacity: 0 }} animate={{ opacity: 1 }} className="text-lg space-y-2">
                <li>🎬 Favourite Movie: Sita Ramam</li>
                <li>🥟 Favourite Food: Momos</li>
                <li>🍫 Favourite Chocolate: Dairy Milk</li>
                <li>💫 Favourite Wearable: Glass Bangles</li>
                <Button onClick={() => setStage("shayari")}>Next</Button>
              </motion.ul>
            )}
          </motion.div>
        )}

        {/* Shayari */}
        {stage === "shayari" && (
          <motion.div className="text-center space-y-6">
            <h2 className="text-3xl font-bold text-rose-600">For You 💝</h2>
            <p className="text-xl italic">
              Tu meri zindagi ki sabse pyari muskaan hai,
              <br />
              Tu har din ko khoobsurat banane wali pehchaan hai,
              <br />
              Tere jaisa dil duniya mein bahut kam hota hai,
              <br />
              Tu sach mein ek bahut special insaan hai 💖
            </p>
            <Button onClick={() => setStage("exit")}>Finish</Button>
          </motion.div>
        )}

        {/* Exit */}
        {stage === "exit" && (
          <motion.div className="text-center space-y-6">
            <h2 className="text-3xl font-bold text-rose-600">Sushma Ji, You Make The World More Beautiful 🌸</h2>
            <p className="text-lg">Some people are rare, pure and magical — you are one of them.</p>
            <div className="text-5xl">🌸💞🌸</div>
          </motion.div>
        )}
      </AnimatePresence>
    </div>
  );
}
