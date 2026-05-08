exdefault function TopNotchDrywallSite() {
  return (
    <div className="min-h-screen bg-black text-white font-sans">
      {/* Navbar */}
      <header className="fixed top-0 w-full bg-black/90 backdrop-blur border-b border-orange-500 z-50">
        <div className="max-w-7xl mx-auto flex items-center justify-between px-6 py-4">
          <div className="flex items-center gap-4">
            <img
              src="/mnt/data/topnotchlogooo.jpg"
              alt="Top Notch Drywall Logo"
              className="w-16 h-16 object-cover rounded-xl border border-orange-500/40"
            />
            <div>
              <h1 className="text-xl font-bold tracking-wide">Top Notch Drywall</h1>
              <p className="text-xs text-gray-400">Professional Drywall Services</p>
            </div>
          </div>

          <nav className="hidden md:flex gap-8 text-sm font-medium">
            <a href="#home" className="hover:text-orange-400 transition">Home</a>
            <a href="#about" className="hover:text-orange-400 transition">About</a>
            <a href="#estimate" className="hover:text-orange-400 transition">Estimate</a>
            <a href="#contact" className="hover:text-orange-400 transition">Contact</a>
          </nav>
        </div>
      </header>

      {/* Hero */}
      <section
        id="home"
        className="relative min-h-screen flex items-center justify-center px-6"
      >
        <div className="absolute inset-0 overflow-hidden">
          <img
            src="/mnt/data/top.jpg"
            alt="Top Notch Drywall Background"
            className="w-full h-full object-cover opacity-40"
          />
          <div className="absolute inset-0 bg-black/70"></div>
        </div>

        <div className="relative z-10 max-w-5xl text-center">
          <img
            src="/mnt/data/topnotchlogooo.jpg"
            alt="Top Notch Drywall Logo"
            className="w-40 md:w-52 mx-auto mb-8 rounded-2xl shadow-2xl border border-orange-500/30"
          />
          <div className="inline-block bg-orange-500/20 border border-orange-500 px-4 py-2 rounded-full text-orange-400 text-sm mb-6">
            The Real Top Notch Drywall in Central Illinois
          </div>

          <h2 className="text-5xl md:text-7xl font-extrabold leading-tight mb-6">
            Quality Work. Top Notch Results.
          </h2>

          <p className="text-lg md:text-xl text-gray-300 max-w-3xl mx-auto mb-10">
            Top Notch Drywall proudly serves Central Illinois with professional drywall repair, hanging, finishing, painting, water damage repair, and remodeling services. We focus on quality workmanship, reliability, and clean professional results for every project.
          </p>

          <div className="flex flex-col sm:flex-row gap-4 justify-center">
            <a
              href="#estimate"
              className="bg-orange-500 hover:bg-orange-400 text-black px-8 py-4 rounded-2xl font-bold transition shadow-lg"
            >
              Request Free Estimate
            </a>

            <a
              href="#contact"
              className="border border-white hover:border-orange-400 hover:text-orange-400 px-8 py-4 rounded-2xl font-bold transition"
            >
              Contact Us
            </a>
          </div>
        </div>
      </section>

      {/* Services */}
      <section className="py-24 px-6 bg-zinc-950">
        <div className="max-w-7xl mx-auto">
          <div className="text-center mb-16">
            <h3 className="text-4xl font-bold mb-4">Our Services</h3>
            <p className="text-gray-400 max-w-2xl mx-auto">
              Residential and commercial drywall solutions completed with
              attention to detail and lasting quality.
            </p>
          </div>

          <div className="grid md:grid-cols-3 gap-8">
            {[
              {
                title: 'Drywall Installation',
                text: 'Professional drywall hanging and installation for new construction and remodeling projects.',
              },
              {
                title: 'Drywall Repair',
                text: 'Fast, seamless repairs for cracks, holes, water damage, and everyday wear and tear.',
              },
              {
                title: 'Finishing & Texture',
                text: 'Smooth finishing, taping, mudding, sanding, and custom texture applications.',
              },
            ].map((service, index) => (
              <div
                key={index}
                className="bg-black border border-zinc-800 hover:border-orange-500 transition rounded-3xl p-8 shadow-xl"
              >
                <div className="w-14 h-14 bg-orange-500 rounded-2xl mb-6"></div>
                <h4 className="text-2xl font-bold mb-4">{service.title}</h4>
                <p className="text-gray-400 leading-relaxed">{service.text}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* About */}
      <section id="about" className="py-24 px-6">
        <div className="max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
          <div>
            <div className="inline-block bg-orange-500/20 border border-orange-500 px-4 py-2 rounded-full text-orange-400 text-sm mb-6">
              About Us
            </div>

            <h3 className="text-5xl font-bold mb-6 leading-tight">
              Built on Quality Work & Professional Service
            </h3>

            <p className="text-gray-300 text-lg leading-relaxed mb-6">
              Top Notch Drywall proudly serves Central Illinois with professional drywall repair, hanging, finishing, painting, water damage repair, and remodeling services. We focus on quality workmanship, reliability, and clean professional results for every project.
            </p>

            <p className="text-gray-400 leading-relaxed mb-8">
              We believe in honest communication, fair pricing, and attention to
              detail from start to finish. Customer satisfaction is always our
              top priority.
            </p>

            <div className="flex gap-8">
              <div>
                <h4 className="text-4xl font-bold text-orange-500">100%</h4>
                <p className="text-gray-400">Customer Focused</p>
              </div>

              <div>
                <h4 className="text-4xl font-bold text-orange-500">Top</h4>
                <p className="text-gray-400">Quality Materials</p>
              </div>
            </div>
          </div>

          <div className="relative">
            <img
              src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?q=80&w=2070&auto=format&fit=crop"
              alt="Drywall Work"
              className="rounded-3xl shadow-2xl border border-orange-500/30"
            />
          </div>
        </div>
      </section>

      {/* Estimate Form */}
      <section id="estimate" className="py-24 px-6 bg-zinc-950">
        <div className="max-w-4xl mx-auto text-center mb-14">
          <h3 className="text-4xl font-bold mb-4">Request a Free Estimate</h3>
          <p className="text-gray-400">
            Tell us about your project and we’ll get back to you as soon as
            possible.
          </p>
        </div>

        <div className="max-w-3xl mx-auto bg-black border border-zinc-800 rounded-3xl p-8 shadow-2xl">
          <form className="grid gap-6">
            <div className="grid md:grid-cols-2 gap-6">
              <input
                type="text"
                placeholder="Full Name"
                className="bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-orange-500"
              />

              <input
                type="email"
                placeholder="Email Address"
                className="bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-orange-500"
              />
            </div>

            <input
              type="tel"
              placeholder="Phone Number"
              className="bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-orange-500"
            />

            <textarea
              rows="6"
              placeholder="Tell us about your project"
              className="bg-zinc-900 border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-orange-500"
            ></textarea>

            <button
              type="submit"
              className="bg-orange-500 hover:bg-orange-400 text-black font-bold py-4 rounded-2xl transition"
            >
              Submit Estimate Request
            </button>
          </form>
        </div>
      </section>

      {/* Contact */}
      <section id="contact" className="py-24 px-6">
        <div className="max-w-5xl mx-auto text-center">
          <div className="inline-block bg-orange-500/20 border border-orange-500 px-4 py-2 rounded-full text-orange-400 text-sm mb-6">
            Contact Us
          </div>

          <h3 className="text-5xl font-bold mb-6">Let’s Build Something Great</h3>

          <p className="text-gray-400 text-lg max-w-2xl mx-auto mb-12">
            Reach out today for drywall services you can count on. We’re ready
            to help with your next project.
          </p>

          <div className="grid md:grid-cols-3 gap-8">
            <div className="bg-zinc-950 border border-zinc-800 rounded-3xl p-8">
              <h4 className="text-xl font-bold mb-2 text-orange-500">Phone</h4>
              <p className="text-gray-400">309-531-6825</p>
            </div>

            <div className="bg-zinc-950 border border-zinc-800 rounded-3xl p-8">
              <h4 className="text-xl font-bold mb-2 text-orange-500">Email</h4>
              <p className="text-gray-400">topnotchdrywall.biz@gmail.com</p>
            </div>

            <div className="bg-zinc-950 border border-zinc-800 rounded-3xl p-8">
              <h4 className="text-xl font-bold mb-2 text-orange-500">Service Area</h4>
              <p className="text-gray-400">Serving Central Illinois</p>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-zinc-800 py-8 px-6 text-center text-gray-500 text-sm">
        © 2026 Top Notch Drywall. All rights reserved.
      </footer>
    </div>
  )
