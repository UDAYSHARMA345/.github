import React from "react";
import { FaCloud, FaShieldAlt, FaLaptopCode, FaPhone } from "react-icons/fa";
import { Button } from "@/components/ui/button";

const Home = () => {
  return (
    <div className="bg-gray-900 text-white min-h-screen">
      {/* Header Section */}
      <header className="py-6 px-8 flex justify-between items-center bg-gray-800 shadow-lg">
        <h1 className="text-3xl font-bold">Nexora Tech</h1>
        <nav>
          <a href="#services" className="px-4">Services</a>
          <a href="#about" className="px-4">About</a>
          <a href="#contact" className="px-4">Contact</a>
        </nav>
      </header>
      
      {/* Hero Section */}
      <section className="text-center py-20 px-10 bg-gradient-to-r from-blue-500 to-purple-600">
        <h2 className="text-5xl font-extrabold">Empowering Businesses with Cutting-Edge IT Solutions</h2>
        <p className="mt-4 text-lg">Innovative cybersecurity, cloud, and IT support solutions tailored to your needs.</p>
        <Button className="mt-6 bg-white text-gray-900 px-6 py-3 font-semibold rounded-lg">Get Started</Button>
      </section>

      {/* Services Section */}
      <section id="services" className="py-16 px-10 text-center">
        <h3 className="text-4xl font-bold mb-6">Our Services</h3>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-10">
          <div className="p-6 bg-gray-800 rounded-lg">
            <FaCloud className="text-blue-400 text-5xl mx-auto" />
            <h4 className="text-2xl mt-4">Cloud Solutions</h4>
            <p>Seamless and scalable cloud computing services for your business.</p>
          </div>
          <div className="p-6 bg-gray-800 rounded-lg">
            <FaShieldAlt className="text-green-400 text-5xl mx-auto" />
            <h4 className="text-2xl mt-4">Cybersecurity</h4>
            <p>Advanced security solutions to protect your data and network.</p>
          </div>
          <div className="p-6 bg-gray-800 rounded-lg">
            <FaLaptopCode className="text-purple-400 text-5xl mx-auto" />
            <h4 className="text-2xl mt-4">IT Support</h4>
            <p>Reliable IT support and troubleshooting for seamless operations.</p>
          </div>
        </div>
      </section>

      {/* About Section */}
      <section id="about" className="py-16 px-10 text-center bg-gray-800">
        <h3 className="text-4xl font-bold mb-6">About Nexora Tech</h3>
        <p className="max-w-3xl mx-auto">Nexora Tech is dedicated to providing cutting-edge IT solutions tailored to modern business needs. Our expertise in cloud services, cybersecurity, and IT support ensures that your company stays secure and efficient.</p>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-16 px-10 text-center">
        <h3 className="text-4xl font-bold mb-6">Get in Touch</h3>
        <p>Have questions? We’re here to help. Reach out to us for IT solutions that fit your business.</p>
        <Button className="mt-6 bg-blue-500 text-white px-6 py-3 font-semibold rounded-lg flex items-center mx-auto">
          <FaPhone className="mr-2" /> Contact Us
        </Button>
      </section>

      {/* Footer */}
      <footer className="py-6 text-center bg-gray-800">
        <p>&copy; 2025 Nexora Tech. All rights reserved.</p>
      </footer>
    </div>
  );
};

export default Home;
