/*
GitHub-Portfolio-React.jsx
A single-file React + Tailwind portfolio component ready to drop into a create-react-app / Vite project.

TOP OF FILE INSTRUCTIONS (CUSTOMIZE BEFORE DEPLOY)
1) Install dependencies:
   npm install react react-dom framer-motion react-icons

2) Tailwind setup (if not already):
   - Follow Tailwind docs for create-react-app or Vite: https://tailwindcss.com/docs/installation
   - Add the Tailwind directives to your main CSS: @tailwind base; @tailwind components; @tailwind utilities;

3) Usage:
   - Place this file as src/Portfolio.jsx
   - Import and render in App.jsx: import Portfolio from './Portfolio'; export default function App(){ return <Portfolio/> }

4) Assets / Replaceables:
   - Replace `PROFILE_IMAGE` with your headshot URL or local import.
   - Replace `projects` array with your real project data and GitHub links.
   - Replace resume.pdf placeholder with a real resume file in public/ or hosting URL.

5) Deploy:
   - For GitHub Pages: follow gh-pages instructions or use GitHub Actions for automatic deploy.
   - For easiest deployment: push to Vercel/Netlify.

README TEMPLATE (copy this to your repo's README.md later):
# Jahnavi Venkata — AI / ML Engineer & Research Enthusiast
> Final-year student passionate about medical AI, deep learning, and machine innovations. Open to internships and collaborative research.

## Highlights
- Research in deep learning and medical imaging
- Implementations with PyTorch and TensorFlow
- Projects: (list 3-5 top projects)

## Contact
- Email: your.email@example.com
- LinkedIn: linkedin.com/in/your
- GitHub: github.com/your

----

*/

import React from 'react';
import { motion } from 'framer-motion';
import { FiMail, FiDownload } from 'react-icons/fi';
import { FaGithub, FaLinkedin, FaTwitter } from 'react-icons/fa';

// Replace this with your profile image URL or import
const PROFILE_IMAGE = 'https://images.unsplash.com/photo-1544005313-94ddf0286df2?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=60';

const projects = [
  {
    title: 'MedScan — Fast Chest X-ray Classifier',
    desc: 'Lightweight CNN with transfer learning for real-time chest X-ray abnormality detection. Includes explainability via Grad-CAM.',
    tags: ['PyTorch', 'Transfer Learning', 'Grad-CAM', 'Docker'],
    repo: '#',
    live: '#'
  },
  {
    title: 'CardioSignal — TinyML Heart Monitor',
    desc: 'Edge-compatible ECG anomaly detection using model compression and pruning for microcontrollers.',
    tags: ['TinyML', 'TensorFlow Lite', 'Quantization'],
    repo: '#',
    live: '#'
  },
  {
    title: 'AutoML-Pipeline',
    desc: 'AutoML orchestration for tabular health records — feature engineering, model selection and monitoring.',
    tags: ['AutoML', 'XGBoost', 'MLflow'],
    repo: '#',
    live: '#'
  }
];

const skills = [
  'Deep Learning (CNN, RNN, Transformers)',
  'PyTorch & TensorFlow',
  'Medical Imaging (DICOM, CT, X-ray)',
  'Model Compression & TinyML',
  'Data Engineering & SQL',
  'Docker, Kubernetes',
  'Research: paper reading and reproducibility',
];

export default function Portfolio(){
  return (
    <div className="min-h-screen bg-gradient-to-br from-gray-900 via-slate-900 to-black text-gray-100 antialiased">
      {/* Decorative animated blobs */}
      <svg className="pointer-events-none absolute inset-0 -z-10 w-full h-full" preserveAspectRatio="none" viewBox="0 0 1200 800">
        <defs>
          <linearGradient id="g1" x1="0" x2="1">
            <stop offset="0%" stopColor="#0ea5e9" stopOpacity="0.12" />
            <stop offset="100%" stopColor="#7c3aed" stopOpacity="0.08" />
          </linearGradient>
        </defs>
        <motion.path
          d="M0 300 C 150 200 300 400 450 300 C 600 200 750 400 900 300 C 1050 200 1200 350 1200 350 L 1200 800 L 0 800 Z"
          fill="url(#g1)"
          initial={{ pathLength: 0 }}
          animate={{ pathLength: 1 }}
          transition={{ duration: 1.8 }}
        />
      </svg>

      <div className="max-w-6xl mx-auto px-6 py-12">
        <header className="flex items-center justify-between mb-10">
          <a href="#" className="flex items-center gap-3">
            <div className="w-12 h-12 rounded-full overflow-hidden ring-2 ring-white/20">
              <img src={PROFILE_IMAGE} alt="profile" className="object-cover w-full h-full" />
            </div>
            <div>
              <h1 className="font-semibold text-lg leading-tight">Jahnavi Venkata</h1>
              <p className="text-xs text-gray-400">AI/ML Engineer · Medical AI · Research Enthusiast</p>
            </div>
          </a>

          <nav className="flex items-center gap-4">
            <a href="#projects" className="text-sm hover:underline">Projects</a>
            <a href="#skills" className="text-sm hover:underline">Skills</a>
            <a href="#about" className="text-sm hover:underline">About</a>
            <a href="#contact" className="text-sm hover:underline">Contact</a>
          </nav>
        </header>

        <main>
          <section className="grid grid-cols-1 md:grid-cols-3 gap-8 items-center mb-12">
            <motion.div className="md:col-span-2 space-y-6"
              initial={{ opacity: 0, x: -30 }}
              animate={{ opacity: 1, x: 0 }}
              transition={{ duration: 0.7 }}
            >
              <h2 className="text-4xl md:text-5xl font-extrabold tracking-tight">AI & ML Engineer — focused on Medical AI</h2>
              <p className="text-lg text-gray-300 max-w-3xl">Final-year student & self-driven researcher building efficient deep-learning models for healthcare. I'm passionate about interpretable models, edge deployment, and turning research into real-world clinical tools. Seeking internships and collaborations in medical AI and embedded ML.</p>

              <div className="flex items-center gap-3">
                <a href="/resume.pdf" className="inline-flex items-center gap-2 bg-white/10 border border-white/10 py-2 px-4 rounded-lg text-sm hover:scale-[1.02] transition">
                  <FiDownload /> Resume
                </a>
                <a href="#projects" className="text-sm text-cyan-300 hover:underline">See my work →</a>
              </div>

              <div className="flex items-center gap-4 mt-2">
                <a aria-label="github" href="#" className="p-3 rounded-lg bg-white/6 hover:bg-white/10 transition"><FaGithub/></a>
                <a aria-label="linkedin" href="#" className="p-3 rounded-lg bg-white/6 hover:bg-white/10 transition"><FaLinkedin/></a>
                <a aria-label="twitter" href="#" className="p-3 rounded-lg bg-white/6 hover:bg-white/10 transition"><FaTwitter/></a>
              </div>
            </motion.div>

            <motion.div className="mx-auto w-60 h-60 rounded-2xl overflow-hidden shadow-2xl ring-1 ring-white/5 bg-gradient-to-b from-white/5 to-white/2 flex items-center justify-center"
              initial={{ scale: 0.9, opacity: 0 }}
              animate={{ scale: 1, opacity: 1 }}
              transition={{ duration: 0.8 }}
            >
              <img src={PROFILE_IMAGE} alt="profile large" className="object-cover w-full h-full" />
            </motion.div>
          </section>

          {/* Projects */}
          <section id="projects" className="mb-12">
            <h3 className="text-2xl font-bold mb-6">Selected projects</h3>
            <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
              {projects.map((p, i) => (
                <motion.article key={p.title}
                  className="bg-gradient-to-tr from-white/3 to-white/2 p-6 rounded-2xl shadow-lg"
                  whileHover={{ scale: 1.03, y: -6 }}
                  transition={{ type: 'spring', stiffness: 200 }}
                >
                  <div className="flex items-start justify-between">
                    <div>
                      <h4 className="text-lg font-semibold">{p.title}</h4>
                      <p className="text-sm text-gray-300 mt-2">{p.desc}</p>
                    </div>
                    <div className="text-xs text-gray-400">#{i+1}</div>
                  </div>

                  <div className="mt-4 flex flex-wrap gap-2">
                    {p.tags.map(t => (
                      <span key={t} className="text-xs bg-white/5 px-2 py-1 rounded-lg">{t}</span>
                    ))}
                  </div>

                  <div className="mt-4 flex items-center gap-3">
                    <a href={p.repo} className="text-sm border border-white/10 px-3 py-2 rounded-lg hover:bg-white/5">Repo</a>
                    <a href={p.live} className="text-sm text-cyan-300 hover:underline">Live</a>
                  </div>
                </motion.article>
              ))}
            </div>
          </section>

          {/* Skills & Timeline */}
          <section id="skills" className="mb-12 grid grid-cols-1 md:grid-cols-2 gap-8">
            <div>
              <h3 className="text-2xl font-bold mb-4">Skills</h3>
              <ul className="space-y-3">
                {skills.map(s => (
                  <li key={s} className="flex items-start gap-3">
                    <motion.span className="w-3 h-3 mt-2 rounded-full bg-cyan-400/80" layout />
                    <div>
                      <div className="font-medium">{s.split(' — ')[0] || s}</div>
                    </div>
                  </li>
                ))}
              </ul>
            </div>

            <div>
              <h3 className="text-2xl font-bold mb-4">Timeline & Research</h3>
              <ol className="border-l border-white/6 pl-4 space-y-6 text-sm text-gray-300">
                <li>
                  <div className="text-xs text-gray-400">2025 — Present</div>
                  <div className="font-semibold">Self-directed research in deep learning for medical imaging</div>
                  <div className="text-gray-400 mt-1">Reproduced SOTA papers, experimented with explainability, and optimized models for edge deployment.</div>
                </li>
                <li>
                  <div className="text-xs text-gray-400">2024</div>
                  <div className="font-semibold">Intern — ML Research</div>
                  <div className="text-gray-400 mt-1">Worked on data curation and model training pipelines for clinical datasets.</div>
                </li>
                <li>
                  <div className="text-xs text-gray-400">2023</div>
                  <div className="font-semibold">Hackathon Winner — MedTech Track</div>
                  <div className="text-gray-400 mt-1">Built a prototype for remote vitals monitoring with TinyML.</div>
                </li>
              </ol>
            </div>
          </section>

          {/* About */}
          <section id="about" className="mb-12">
            <h3 className="text-2xl font-bold mb-4">About me</h3>
            <div className="bg-white/3 p-6 rounded-2xl text-gray-200">
              <p className="mb-3">I'm a final-year engineering student building research-grade deep learning systems for healthcare. My work focuses on model interpretability, domain-specific data handling (DICOM), and deployment constraints for clinical environments. When I'm not coding I read research papers, tinker with embedded systems, and mentor juniors.</p>

              <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                <div>
                  <p className="text-sm text-gray-300">Preferred tech stack</p>
                  <ul className="text-sm mt-2">
                    <li>PyTorch · OpenCV · DICOM</li>
                    <li>TensorFlow Lite · Edge Impulse</li>
                    <li>Docker · MLflow · Airflow</li>
                  </ul>
                </div>

                <div>
                  <p className="text-sm text-gray-300">Open to</p>
                  <ul className="text-sm mt-2">
                    <li>Internships in Medical AI / Research roles</li>
                    <li>Collaborations on reproducible research</li>
                    <li>Open-source contributions</li>
                  </ul>
                </div>
              </div>
            </div>
          </section>

          {/* Contact */}
          <section id="contact" className="mb-20">
            <h3 className="text-2xl font-bold mb-4">Contact</h3>
            <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
              <div className="md:col-span-2 bg-white/4 p-6 rounded-2xl">
                <form action={`mailto:your.email@example.com`} method="post" encType="text/plain">
                  <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <input name="name" placeholder="Your name" className="p-3 rounded-lg bg-white/5 border border-white/6" />
                    <input name="email" placeholder="Your email" className="p-3 rounded-lg bg-white/5 border border-white/6" />
                    <input name="subject" placeholder="Subject" className="p-3 rounded-lg bg-white/5 border border-white/6 md:col-span-2" />
                    <textarea name="message" placeholder="Message" className="p-3 rounded-lg bg-white/5 border border-white/6 md:col-span-2 h-28"></textarea>
                  </div>

                  <div className="mt-4 flex items-center gap-3">
                    <button type="submit" className="inline-flex items-center gap-2 bg-cyan-500 text-black px-4 py-2 rounded-lg font-medium">Send message <FiMail/></button>
                    <a href="mailto:your.email@example.com" className="text-sm text-gray-300">Or email: your.email@example.com</a>
                  </div>
                </form>
              </div>

              <div className="bg-white/3 p-6 rounded-2xl flex flex-col gap-4 text-sm">
                <div>
                  <div className="text-xs text-gray-300">Current location</div>
                  <div className="font-medium">India</div>
                </div>

                <div>
                  <div className="text-xs text-gray-300">Open to</div>
                  <div className="font-medium">Internships / Research collaborations</div>
                </div>

                <div>
                  <div className="text-xs text-gray-300">Available for</div>
                  <div className="font-medium">Remote & On-site</div>
                </div>
              </div>
            </div>
          </section>

        </main>

        <footer className="text-center text-sm text-gray-400 py-6">Made with ❤️ • Built for research, reproducibility & deployment • <a href="#" className="underline">GitHub</a></footer>
      </div>
    </div>
  );
}
