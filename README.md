import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { motion } from "framer-motion";

export default function Home() {
  return (
    <main className="min-h-screen bg-black text-white px-4 py-8">
      <motion.div
        initial={{ opacity: 0, y: -20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.8 }}
        className="text-center mb-10"
      >
        <h1 className="text-4xl font-bold mb-2">VisioGen Graphics</h1>
        <p className="text-lg text-gray-400">
          Bringing Visions to Life | Design. Motion. Innovation.
        </p>
      </motion.div>
      <section className="grid md:grid-cols-2 gap-6">
        <Card className="bg-gray-900 rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Logo Design</h2>
            <p className="text-gray-400 mb-4">
              Unique logos that define your brand identity.
            </p>
            <Button variant="outline" className="border-white text-white">
              View Work
            </Button>
          </CardContent>
        </Card>
        <Card className="bg-gray-900 rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Brochures & Pamphlets</h2>
            <p className="text-gray-400 mb-4">
              Modern layouts that captivate your audience.
            </p>
            <Button variant="outline" className="border-white text-white">
              View Work
            </Button>
          </CardContent>
        </Card>
        <Card className="bg-gray-900 rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">T-Shirt Graphics</h2>
            <p className="text-gray-400 mb-4">
              Custom apparel designs for your brand or event.
            </p>
            <Button variant="outline" className="border-white text-white">
              View Work
            </Button>
          </CardContent>
        </Card>
        <Card className="bg-gray-900 rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Cinematography & Video</h2>
            <p className="text-gray-400 mb-4">
              High-quality visuals and storytelling for your brand.
            </p>
            <Button variant="outline" className="border-white text-white">
              View Work
            </Button>
          </CardContent>
        </Card>
      </section>
      <motion.footer
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.5, duration: 1 }}
        className="text-center mt-16 text-sm text-gray-500"
      >
        © 2025 VisioGen Graphics | contact@visiogengraphics.com
      </motion.footer>
    </main>
  );
}
