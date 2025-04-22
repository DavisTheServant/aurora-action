import React from "react";

function App() {
  return (
    <div className="min-h-screen bg-gray-50 text-gray-800">
      {/* Hero Section */}
      <header className="bg-blue-600 text-white py-20 text-center">
        <h1 className="text-4xl md:text-5xl font-bold">Davis Computer Skills</h1>
        <p className="mt-4 text-lg md:text-xl">Learn the skills that power the digital world.</p>
        <a
          href="#courses"
          className="mt-6 inline-block bg-white text-blue-600 px-6 py-3 rounded-full font-semibold hover:bg-blue-100 transition"
        >
          Browse Courses
        </a>
      </header>

      {/* Why Choose Us */}
      <section className="py-16 px-6 text-center">
        <h2 className="text-3xl font-bold mb-8">Why Choose Us?</h2>
        <div className="grid md:grid-cols-4 gap-6">
          {["Hands-on Training", "Beginner-Friendly", "Job-Ready Skills", "Flexible Learning"].map(
            (feature, i) => (
              <div
                key={i}
                className="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition"
              >
                <p className="text-lg font-semibold">{feature}</p>
              </div>
            )
          )}
        </div>
      </section>

      {/* Featured Courses */}
      <section id="courses" className="py-16 px-6 bg-gray-100">
        <h2 className="text-3xl font-bold text-center mb-10">Featured Courses</h2>
        <div className="grid md:grid-cols-3 gap-6">
          {[
            { title: "Basic Computer Skills", desc: "Perfect for absolute beginners." },
            { title: "IT Fundamentals", desc: "PC building, networks, and troubleshooting." },
            { title: "Software Development", desc: "Learn to code using real-world projects." },
          ].map((course, i) => (
            <div
              key={i}
              className="bg-white p-6 rounded-2xl shadow hover:shadow-lg transition"
            >
              <h3 className="text-xl font-semibold mb-2">{course.title}</h3>
              <p>{course.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* CTA Section */}
      <section className="py-20 text-center bg-blue-600 text-white">
        <h2 className="text-3xl font-bold">Ready to level up your skills?</h2>
        <p className="mt-4">Enroll today and start learning tomorrow.</p>
        <a
          href="#contact"
          className="mt-6 inline-block bg-white text-blue-600 px-6 py-3 rounded-full font-semibold hover:bg-blue-100 transition"
        >
          Enroll Now
        </a>
      </section>

      {/* Footer */}
      <footer id="contact" className="bg-gray-800 text-white text-center py-10">
        <p>Davis Computer Skills &copy; 2025 | 123 Tech Ave | (801) 555-1234</p>
        <p className="text-sm">Email: info@daviscomputerskills.com</p>
      </footer>
    </div>
  );
}

export default App;
