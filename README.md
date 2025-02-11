# repository1
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Linkedin } from "lucide-react";

export default function Home() {
  return (
    <div className="min-h-screen bg-gray-100 flex flex-col items-center p-6">
      {/* Header */}
      <header className="text-center py-10">
        <h1 className="text-4xl font-bold text-gray-900">Louis Lopez</h1>
        <p className="text-lg text-gray-600">Consultant | Economist | Aspiring Thought Leader</p>
      </header>
      
      {/* About Section */}
      <Card className="max-w-2xl w-full bg-white shadow-lg rounded-2xl p-6 mb-6">
        <CardContent>
          <h2 className="text-2xl font-semibold mb-3">About Me</h2>
          <p className="text-gray-700">
            I'm a consultant at BCG with a deep passion for finance, economics, and policy. 
            Through my research, writing, and projects, I aim to contribute to discussions on 
            private equity, macroeconomics, and long-term economic trends.
          </p>
        </CardContent>
      </Card>
      
      {/* Thought Leadership Section */}
      <Card className="max-w-2xl w-full bg-white shadow-lg rounded-2xl p-6 mb-6">
        <CardContent>
          <h2 className="text-2xl font-semibold mb-3">Thought Leadership</h2>
          <p className="text-gray-700">
            Exploring topics like demographic risk, macroeconomic shifts, and the future of private equity.
            Read my latest insights on economic transformations and financial markets.
          </p>
        </CardContent>
      </Card>
      
      {/* Contact Section */}
      <Card className="max-w-2xl w-full bg-white shadow-lg rounded-2xl p-6 mb-6 text-center">
        <CardContent>
          <h2 className="text-2xl font-semibold mb-3">Get in Touch</h2>
          <p className="text-gray-700 mb-4">Feel free to reach out for collaborations, discussions, or inquiries.</p>
          <div className="flex justify-center gap-4">
            <Button variant="outline">
              <Mail className="mr-2" /> Email Me
            </Button>
            <Button variant="outline">
              <Linkedin className="mr-2" /> Connect on LinkedIn
            </Button>
          </div>
        </CardContent>
      </Card>
    </div>
  );
}
