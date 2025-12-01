rofile-Animated-Portfolio.jsx
{ title: 'AutoML-Pipeline', desc: 'Automated ML for health records', tags: ['AutoML','XGBoost','MLflow'], repo: '#', live: '#', icon: <FaMicroscope /> },
{ title: 'BrainInnovator', desc: 'Research-driven AI exploration', tags: ['Deep Learning','Transformers'], repo: '#', live: '#', icon: <FaBrain /> }
];


const skills = ['Deep Learning', 'Medical AI', 'PyTorch & TensorFlow', 'TinyML & Edge AI', 'Data Engineering', 'Model Explainability', 'Docker & MLflow'];


export default function GitHubPortfolio(){
return (
<div className="min-h-screen bg-gradient-to-br from-gray-900 via-slate-900 to-black text-gray-100 antialiased">
<motion.div className="max-w-5xl mx-auto px-6 py-12 text-center"
initial={{ opacity:0 }} animate={{ opacity:1 }} transition={{ duration:1 }}>
<motion.h1 className="text-5xl font-extrabold mb-4" animate={{ scale:[1,1.05,1] }} transition={{ duration:1.5, repeat: Infinity }}>Hello! Jahnavi in the house 👋</motion.h1>
<p className="text-lg text-gray-300 mb-6">Motivated by helping those in need, exploring new innovations, conducting research, and applying AI/ML in the health industry. Passionate to experience the thrill of science and deep learning explorations.</p>
<div className="flex justify-center gap-4 mb-8">
<a href="#projects" className="px-4 py-2 bg-cyan-500 rounded-lg font-medium hover:scale-105 transition">Explore Projects</a>
<a href="/resume.pdf" className="px-4 py-2 bg-white/10 rounded-lg font-medium flex items-center gap-2 hover:scale-105 transition"><FiDownload /> Resume</a>
</div>
<div className="flex justify-center gap-4 text-2xl mb-12">
<a href="#" className="hover:text-cyan-400"><FaGithub /></a>
<a href="#" className="hover:text-blue-500"><FaLinkedin /></a>
<a href="#" className="hover:text-blue-400"><FaTwitter /></a>
</div>


<section id="projects" className="space-y-6">
<h2 className="text-3xl font-bold mb-4">Projects & Research</h2>
<div className="grid md:grid-cols-2 gap-6">
{projects.map((p,i)=>(
<motion.div key={i} whileHover={{ scale:1.03, y:-5 }} className="bg-white/5 p-6 rounded-2xl shadow-lg flex gap-4 items-start">
<div className="text-cyan-400 text-3xl mt-1">{p.icon}</div>
<div>
<h3 className="text-xl font-semibold mb-2">{p.title}</h3>
<p className="text-gray-300 mb-2">{p.desc}</p>
<div className="flex flex-wrap gap-2 mb-2">{p.tags.map(t=><span key={t} className="text-xs bg-white/10 px-2 py-1 rounded-lg">{t}</span>)}</div>
<div className="flex gap-3 text-sm">
<a href={p.repo} className="border border-white/20 px-2 py-1 rounded-lg hover:bg-white/10">Repo</a>
<a href={p.live} className="text-cyan-400 hover:underline">Live</a>
</div>
</div>
</motion.div>
))}
</div>
</section>


<section id="skills" className="mt-12">
<h2 className="text-3xl font-bold mb-4">Skills & Expertise</h2>
<div className="flex flex-wrap gap-3 justify-center">
{skills.map(s=><span key={s} className="bg-white/10 px-3 py-1 rounded-full text-sm hover:bg-cyan-500 transition cursor-default">{s}</span>)}
</div>
</section>
</motion.div>


<footer className="text-center text-sm text-gray-400 py-6">Made with ❤️ • Exploring AI/ML in health & science • GitHub-ready portfolio</footer>
</div>
);
}
