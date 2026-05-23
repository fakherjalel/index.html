# index.html
export default function PortfolioWebsite() {
  const whatsappNumber = "21600000000";

  const projectLinks = {
    "Cinematic Reels": "https://www.instagram.com/fakher.7x/",
    "Personal Branding": "https://www.instagram.com/fakher.7x/",
    "Product Commercials": "https://www.instagram.com/fakher.7x/",
  };

  const serviceLinks = {
    "Short Form Video Editing": `https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20need%20short-form%20video%20editing`,
    "Personal Brand Content": `https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20want%20personal%20brand%20content`,
    "Motion Graphics": `https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20need%20motion%20graphics`,
    "TikTok / Reels Strategy": `https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20need%20TikTok%20strategy`,
    "YouTube Editing": `https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20need%20YouTube%20editing`,
    "Cinematic Color Grading": `https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20need%20cinematic%20color%20grading`,
  };

  const projects = [
    {
      title: "Cinematic Reels",
      description: "High-retention short form edits for creators and brands.",
      stats: "2M+ Views",
    },
    {
      title: "Personal Branding",
      description: "Professional talking-head content designed to convert viewers into clients.",
      stats: "30+ Clients",
    },
    {
      title: "Product Commercials",
      description: "Fast-paced commercial edits with cinematic lighting and motion graphics.",
      stats: "4x Engagement",
    },
  ];

  const services = [
    "Short Form Video Editing",
    "Personal Brand Content",
    "Motion Graphics",
    "TikTok / Reels Strategy",
    "YouTube Editing",
    "Cinematic Color Grading",
  ];

  return (
    <div className="min-h-screen bg-black text-white font-sans overflow-x-hidden">
      {/* HERO */}
      <section className="relative min-h-screen flex items-center justify-center px-6">
        <div className="absolute inset-0 bg-gradient-to-b from-zinc-900 via-black to-black" />

        <div className="relative z-10 max-w-6xl w-full grid lg:grid-cols-2 gap-14 items-center">
          <div>
            <div className="inline-flex items-center gap-2 border border-zinc-700 bg-zinc-900/60 px-4 py-2 rounded-full text-sm mb-6">
              <div className="w-2 h-2 rounded-full bg-green-400 animate-pulse" />
              Available for freelance work
            </div>

            <h1 className="text-5xl md:text-7xl font-black leading-tight tracking-tight">
              I Create
              <span className="block text-zinc-400">Viral Content</span>
              That Gets Attention.
            </h1>

            <p className="mt-6 text-zinc-400 text-lg max-w-xl leading-relaxed">
              Freelance video editor & content creator helping brands and creators
              grow through cinematic storytelling, high-retention editing and
              powerful personal branding.
            </p>

            <div className="flex flex-wrap gap-4 mt-10">
              <a
                href="#projects"
                className="px-7 py-4 rounded-2xl bg-white text-black font-semibold hover:scale-105 transition-transform"
              >
                View Projects
              </a>

              <a
                href={`https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20want%20to%20work%20with%20you`}
                target="_blank"
                rel="noopener noreferrer"
                className="px-7 py-4 rounded-2xl border border-zinc-700 hover:bg-zinc-900 transition-colors"
              >
                Contact Me
              </a>
            </div>
          </div>

          <div className="relative flex justify-center">
            <div className="absolute w-72 h-72 bg-white/10 blur-3xl rounded-full" />

            <div className="relative bg-zinc-900 border border-zinc-800 rounded-[32px] p-4 shadow-2xl w-full max-w-md">
              <img
                src="https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?q=80&w=1200&auto=format&fit=crop"
                alt="creator"
                className="rounded-[24px] h-[500px] object-cover w-full"
              />

              <div className="absolute bottom-8 left-8 right-8 bg-black/70 backdrop-blur-xl border border-zinc-800 rounded-2xl p-4">
                <div className="flex items-center justify-between">
                  <div>
                    <h3 className="font-bold text-lg">Freelance Creator</h3>
                    <p className="text-zinc-400 text-sm">Video Editing • Branding</p>
                  </div>

                  <div className="text-right">
                    <p className="font-bold text-2xl">24/7</p>
                    <p className="text-zinc-500 text-sm">Creative Workflow</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* STATS */}
      <section className="px-6 py-20 border-y border-zinc-900 bg-zinc-950">
        <div className="max-w-6xl mx-auto grid grid-cols-2 md:grid-cols-4 gap-6 text-center">
          {[
            ["50+", "Projects Completed"],
            ["10M+", "Total Views"],
            ["95%", "Client Satisfaction"],
            ["24h", "Fast Delivery"],
          ].map(([number, label]) => (
            <div
              key={label}
              className="bg-black border border-zinc-800 rounded-3xl p-8"
            >
              <h3 className="text-4xl font-black">{number}</h3>
              <p className="text-zinc-500 mt-2">{label}</p>
            </div>
          ))}
        </div>
      </section>

      {/* PROJECTS */}
      <section id="projects" className="px-6 py-28">
        <div className="max-w-6xl mx-auto">
          <div className="mb-16">
            <p className="text-zinc-500 uppercase tracking-[0.3em] text-sm">
              Portfolio
            </p>
            <h2 className="text-5xl font-black mt-4">Featured Work</h2>
          </div>

          <div className="grid md:grid-cols-3 gap-8">
            {projects.map((project) => (
              <a
                key={project.title}
                href={projectLinks[project.title]}
                target="_blank"
                rel="noopener noreferrer"
                className="block"
              >
                <div className="group bg-zinc-950 border border-zinc-800 rounded-[32px] overflow-hidden hover:-translate-y-2 transition-all duration-300 cursor-pointer hover:border-white">
                  <div className="h-72 overflow-hidden">
                    <img
                      src="https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?q=80&w=1200&auto=format&fit=crop"
                      alt={project.title}
                      className="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                    />
                  </div>

                  <div className="p-8">
                    <div className="flex items-center justify-between mb-4">
                      <h3 className="text-2xl font-bold">{project.title}</h3>
                      <span className="text-sm px-3 py-1 rounded-full bg-zinc-900 border border-zinc-700 text-zinc-300">
                        {project.stats}
                      </span>
                    </div>

                    <p className="text-zinc-400 leading-relaxed">
                      {project.description}
                    </p>
                  </div>
                </div>
              </a>
            ))}
          </div>
        </div>
      </section>

      {/* SERVICES */}
      <section className="px-6 py-28 bg-zinc-950 border-y border-zinc-900">
        <div className="max-w-6xl mx-auto grid lg:grid-cols-2 gap-14 items-start">
          <div>
            <p className="text-zinc-500 uppercase tracking-[0.3em] text-sm">
              Services
            </p>

            <h2 className="text-5xl font-black mt-4 leading-tight">
              Everything You Need
              <span className="block text-zinc-400">To Grow Online</span>
            </h2>
          </div>

          <div className="grid gap-4">
            {services.map((service) => (
              <a
                key={service}
                href={serviceLinks[service]}
                target="_blank"
                rel="noopener noreferrer"
              >
                <div className="bg-black border border-zinc-800 rounded-2xl p-6 flex items-center justify-between hover:border-white transition-all duration-300 cursor-pointer hover:scale-[1.02]">
                  <span className="text-lg">{service}</span>
                  <span className="text-zinc-500">→</span>
                </div>
              </a>
            ))}
          </div>
        </div>
      </section>

      {/* CTA */}
      <section className="px-6 py-32">
        <div className="max-w-4xl mx-auto text-center bg-zinc-950 border border-zinc-800 rounded-[40px] p-14">
          <p className="text-zinc-500 uppercase tracking-[0.3em] text-sm">
            Let's Work
          </p>

          <h2 className="text-5xl md:text-6xl font-black mt-6 leading-tight">
            Ready To Build
            <span className="block text-zinc-400">Your Brand?</span>
          </h2>

          <p className="text-zinc-400 mt-6 max-w-2xl mx-auto text-lg leading-relaxed">
            Whether you need viral short-form content, cinematic edits or a full
            personal branding strategy — I can help you stand out online.
          </p>

          <div className="flex flex-wrap justify-center gap-4 mt-10">
            <a
              href={`https://wa.me/${whatsappNumber}?text=Hey%20Fakher%2C%20I%20want%20to%20start%20a%20project`}
              target="_blank"
              rel="noopener noreferrer"
              className="px-8 py-4 bg-white text-black rounded-2xl font-bold hover:scale-105 transition-transform"
            >
              Start A Project
            </a>

            <a
              href="https://www.instagram.com/fakher.7x/?utm_source=ig_web_button_share_sheet"
              target="_blank"
              rel="noopener noreferrer"
              className="px-8 py-4 border border-zinc-700 rounded-2xl hover:bg-zinc-900 transition-colors"
            >
              Instagram
            </a>
          </div>
        </div>
      </section>
    </div>
  );
}
