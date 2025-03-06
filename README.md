import React from "react";
import { motion } from "framer-motion";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

const sections = {
  "Lorena R7": [
    {
      title: "Título do Texto 1",
      description: "Descrição breve do texto 1...",
      link: "#",
    },
    {
      title: "Título do Texto 2",
      description: "Descrição breve do texto 2...",
      link: "#",
    },
  ],
  "In Magazine": [
    {
      title: "Título do Texto 3",
      description: "Descrição breve do texto 3...",
      link: "#",
    },
    {
      title: "Título do Texto 4",
      description: "Descrição breve do texto 4...",
      link: "#",
    },
  ],
  "Prensa": [
    {
      title: "Título do Texto 5",
      description: "Descrição breve do texto 5...",
      link: "#",
    },
  ],
  "Prefeitura Praia Grande": [
    {
      title: "Título do Texto 6",
      description: "Descrição breve do texto 6...",
      link: "#",
    },
  ],
  "Câmara de Cubatão": [
    {
      title: "Título do Texto 7",
      description: "Descrição breve do texto 7...",
      link: "#",
    },
  ],
};

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gradient-to-r from-blue-500 to-purple-600 p-8 text-white">
      <motion.h1
        className="text-4xl font-bold text-center mb-8"
        initial={{ opacity: 0, y: -20 }}
        animate={{ opacity: 1, y: 0 }}
      >
        Portfólio Rafaela Ribeiro
      </motion.h1>
      
      {Object.entries(sections).map(([section, articles], secIndex) => (
        <div key={secIndex} className="mb-10">
          <h2 className="text-2xl font-semibold mb-4">{section}</h2>
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
            {articles.map((article, index) => (
              <motion.div
                key={index}
                initial={{ opacity: 0, scale: 0.9 }}
                animate={{ opacity: 1, scale: 1 }}
                transition={{ delay: index * 0.2 }}
              >
                <Card className="bg-white text-black rounded-2xl shadow-lg overflow-hidden">
                  <CardContent className="p-6">
                    <h2 className="text-xl font-semibold mb-2">{article.title}</h2>
                    <p className="text-sm mb-4">{article.description}</p>
                    <Button asChild>
                      <a href={article.link} target="_blank" rel="noopener noreferrer">
                        Ler mais
                      </a>
                    </Button>
                  </CardContent>
                </Card>
              </motion.div>
            ))}
          </div>
        </div>
      ))}
    </div>
  );
}

