import { motion } from "framer-motion"; import { Card, CardContent } from "@/components/ui/card"; import { Cake, Heart, Sparkles } from "lucide-react";

export default function BirthdayWebsite() { return ( <div className="min-h-screen bg-gradient-to-br from-pink-200 via-purple-200 to-indigo-200 flex items-center justify-center p-4"> <motion.div initial={{ opacity: 0, scale: 0.8 }} animate={{ opacity: 1, scale: 1 }} transition={{ duration: 1 }} className="max-w-md w-full" > <Card className="rounded-2xl shadow-2xl bg-white/80 backdrop-blur"> <CardContent className="p-6 text-center space-y-4"> <motion.h1 initial={{ y: -30, opacity: 0 }} animate={{ y: 0, opacity: 1 }} transition={{ delay: 0.5 }} className="text-3xl font-bold text-pink-600" > 🎉 Happy Birthday Simran 🎉 </motion.h1>

<motion.img
          src="https://via.placeholder.com/300x300.png?text=Simran+Photo"
          alt="Simran"
          className="w-48 h-48 mx-auto rounded-full object-cover border-4 border-pink-400 shadow-lg"
          initial={{ scale: 0 }}
          animate={{ scale: 1 }}
          transition={{ delay: 0.8, type: "spring" }}
        />

        <motion.p
          initial={{ opacity: 0 }}
          animate={{ opacity: 1 }}
          transition={{ delay: 1.2 }}
          className="text-gray-700"
        >
          Dear Simran 💖<br />
          May your life be filled with happiness, smiles, love and success.
          You are very special and today is all about you ✨
        </motion.p>

        <motion.div
          className="flex justify-center gap-4 text-pink-500"
          initial={{ opacity: 0 }}
          animate={{ opacity: 1 }}
          transition={{ delay: 1.5 }}
        >
          <Cake />
          <Heart />
          <Sparkles />
        </motion.div>

        <motion.p
          initial={{ y: 20, opacity: 0 }}
          animate={{ y: 0, opacity: 1 }}
          transition={{ delay: 1.8 }}
          className="text-sm text-gray-600"
        >
          With lots of love 💕<br />
          — From your brother
        </motion.p>
      </CardContent>
    </Card>
  </motion.div>
</div>

); }
