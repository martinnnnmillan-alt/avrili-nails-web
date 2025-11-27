import React, { useState, useEffect, useRef } from 'react';
import { 
  Heart, Star, Calendar, ShoppingBag, Menu, X, Instagram, 
  MapPin, Phone, Mail, ChevronRight, CheckCircle, Sun, Moon,
  Sparkles, Clock, ShieldCheck, Trash2, Plus, Minus
} from 'lucide-react';
import { motion, AnimatePresence } from 'framer-motion';

// --- DATA & CONTENT ---

const BRAND = {
  name: "Avrili Nails",
  owner: "Delfii Vazquez",
  slogan: "Tus uñas, tu mejor accesorio.",
  instagram: "@avrili_nails",
  colors: {
    primary: "pink-500", // Tailwind class reference
    secondary: "black"
  }
};

const SERVICES = [
  {
    id: 1,
    title: "Esculpidas Premium",
    price: "$18.000",
    time: "2.5 hs",
    desc: "Extensiones artificiales creadas desde cero con polímero o gel de construcción, adaptadas a la anatomía de tu uña natural.",
    benefits: ["Durabilidad extrema (20-30 días)", "Corrección de uñas mordidas", "Largo y forma totalmente personalizable"],
    includes: "Manicura rusa combinada + Esculpido + Esmaltado liso + Hidratación de cutículas.",
    img: "https://images.unsplash.com/photo-1604654894610-df63bc536371?auto=format&fit=crop&q=80&w=800"
  },
  {
    id: 2,
    title: "Soft Gel / Capping",
    price: "$14.000",
    time: "1.5 hs",
    desc: "Sistema innovador de tips de gel que cubren toda la uña o capa protectora sobre tu largo natural.",
    benefits: ["Apariencia súper natural", "Flexible y resistente", "Ideal para dejar crecer tu uña"],
    includes: "Preparación de la uña + Aplicación Soft Gel/Capping + Esmaltado semipermanente.",
    img: "https://images.unsplash.com/photo-1632922267756-9b71242b1592?auto=format&fit=crop&q=80&w=800"
  },
  {
    id: 3,
    title: "Nail Art Personalizado",
    price: "Desde $2.000",
    time: "+30 min",
    desc: "Arte a mano alzada, encapsulados, pedrería y diseños 3D inspirados en tu estilo único.",
    benefits: ["Diseños exclusivos", "Tendencias virales (Y2K, Coquette, Cyber)", "Personalización total"],
    includes: "Diseño por uña o set completo (consultar complejidad).",
    img: "https://images.unsplash.com/photo-1522337360705-8754d8722b39?auto=format&fit=crop&q=80&w=800"
  },
  {
    id: 4,
    title: "Press-On Nails",
    price: "$10.000",
    time: "Envío inmediato",
    desc: "Uñas reutilizables hechas a medida. La calidad del salón en la comodidad de tu casa.",
    benefits: ["Reutilizables", "Se ponen en 10 minutos", "No dañan tu uña natural"],
    includes: "Set de 10 uñas + Kit de aplicación (lima, palito, pegamento/tabs, toallita).",
    img: "https://images.unsplash.com/photo-1599693988002-3932e675034c?auto=format&fit=crop&q=80&w=800"
  },
  {
    id: 5,
    title: "Spa de Manos & Pies",
    price: "$8.500",
    time: "1 hs",
    desc: "Tratamiento de hidratación profunda y exfoliación para rejuvenecer la piel de tus manos y pies.",
    benefits: ["Piel suave y luminosa", "Relajación total", "Mejora la circulación"],
    includes: "Exfoliación + Mascarilla + Masaje + Esmaltado tradicional o nutrición.",
    img: "https://images.unsplash.com/photo-1519014816548-bf5fe059e98b?auto=format&fit=crop&q=80&w=800"
  }
];

const PRODUCTS = [
  { id: 101, name: "Set Press-On 'Baddie' XL", price: 12500, category: "Press-On", img: "https://images.unsplash.com/photo-1632922267756-9b71242b1592?auto=format&fit=crop&q=80&w=400" },
  { id: 102, name: "Aceite de Cutículas Avrili", price: 3500, category: "Cuidado", img: "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&q=80&w=400" },
  { id: 103, name: "Kit de Retiro Seguro", price: 5000, category: "Herramientas", img: "https://images.unsplash.com/photo-1596462502278-27bfdd403ea2?auto=format&fit=crop&q=80&w=400" },
  { id: 104, name: "Set Press-On 'Coquette'", price: 12500, category: "Press-On", img: "https://images.unsplash.com/photo-1522337660859-02fbefca4702?auto=format&fit=crop&q=80&w=400" },
];

const REVIEWS = [
  { id: 1, name: "Martina G.", text: "Las mejores esculpidas que me hice. Delfi es súper detallista y el lugar es hermoso.", rating: 5, img: "https://randomuser.me/api/portraits/women/44.jpg" },
  { id: 2, name: "Sofi L.", text: "Pedí unas Press-On personalizadas y llegaron impecables, el packaging es un sueño.", rating: 5, img: "https://randomuser.me/api/portraits/women/68.jpg" },
  { id: 3, name: "Camila R.", text: "Amo el nail art que hace, le llevé un diseño re difícil y lo hizo igual.", rating: 5, img: "https://randomuser.me/api/portraits/women/12.jpg" },
];

// --- COMPONENTS ---

// 1. Navigation
const Navbar = ({ cartCount, toggleCart, darkMode, toggleTheme, scrollToSection }) => {
  const [isOpen, setIsOpen] = useState(false);
  const [scrolled, setScrolled] = useState(false);

  useEffect(() => {
    const handleScroll = () => setScrolled(window.scrollY > 50);
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, []);

  const navLinks = [
    { name: 'Inicio', target: 'home' },
    { name: 'Servicios', target: 'services' },
    { name: 'Tienda', target: 'shop' },
    { name: 'Galería', target: 'gallery' },
    { name: 'Reservar', target: 'booking' },
    { name: 'Nosotros', target: 'about' },
  ];

  return (
    <nav className={`fixed w-full z-50 transition-all duration-300 ${scrolled ? 'bg-white/90 dark:bg-zinc-900/90 backdrop-blur-md shadow-md py-2' : 'bg-transparent py-4'}`}>
      <div className="container mx-auto px-6 flex justify-between items-center">
        {/* Logo */}
        <div 
          onClick={() => scrollToSection('home')}
          className="cursor-pointer flex items-center gap-2 group"
        >
          <div className="relative">
            <div className="w-10 h-10 bg-pink-500 rounded-full flex items-center justify-center text-white border-2 border-black dark:border-white">
               <Heart size={20} fill="white" />
            </div>
            <div className="absolute -bottom-1 -right-1 bg-black text-white text-[8px] px-1 rounded-sm font-bold">AV</div>
          </div>
          <span className="font-serif text-xl font-bold tracking-wide text-zinc-800 dark:text-white group-hover:text-pink-500 transition-colors">
            Avrili<span className="text-pink-500">Nails</span>
          </span>
        </div>

        {/* Desktop Menu */}
        <div className="hidden md:flex items-center gap-8">
          {navLinks.map((link) => (
            <button 
              key={link.name} 
              onClick={() => scrollToSection(link.target)}
              className="text-sm font-medium text-zinc-600 dark:text-zinc-300 hover:text-pink-500 dark:hover:text-pink-400 transition-colors uppercase tracking-wider"
            >
              {link.name}
            </button>
          ))}
        </div>

        {/* Icons */}
        <div className="flex items-center gap-4">
          <button onClick={toggleTheme} className="p-2 rounded-full hover:bg-zinc-100 dark:hover:bg-zinc-800 text-zinc-600 dark:text-zinc-300 transition-colors">
            {darkMode ? <Sun size={20} /> : <Moon size={20} />}
          </button>
          
          <button onClick={toggleCart} className="relative p-2 rounded-full hover:bg-zinc-100 dark:hover:bg-zinc-800 text-zinc-600 dark:text-zinc-300 transition-colors">
            <ShoppingBag size={20} />
            {cartCount > 0 && (
              <span className="absolute top-0 right-0 bg-pink-500 text-white text-xs w-4 h-4 rounded-full flex items-center justify-center font-bold animate-bounce">
                {cartCount}
              </span>
            )}
          </button>

          <button onClick={() => setIsOpen(!isOpen)} className="md:hidden p-2 text-zinc-800 dark:text-white">
            {isOpen ? <X size={24} /> : <Menu size={24} />}
          </button>
        </div>
      </div>

      {/* Mobile Menu */}
      <AnimatePresence>
        {isOpen && (
          <motion.div 
            initial={{ opacity: 0, height: 0 }}
            animate={{ opacity: 1, height: 'auto' }}
            exit={{ opacity: 0, height: 0 }}
            className="md:hidden bg-white dark:bg-zinc-900 border-t dark:border-zinc-800"
          >
            <div className="flex flex-col p-6 gap-4">
              {navLinks.map((link) => (
                <button 
                  key={link.name} 
                  onClick={() => {
                    scrollToSection(link.target);
                    setIsOpen(false);
                  }}
                  className="text-left text-lg font-medium text-zinc-800 dark:text-zinc-200"
                >
                  {link.name}
                </button>
              ))}
            </div>
          </motion.div>
        )}
      </AnimatePresence>
    </nav>
  );
};

// 2. Hero Section
const Hero = ({ scrollToSection }) => {
  return (
    <section id="home" className="relative h-screen flex items-center justify-center overflow-hidden">
      {/* Background Image with Overlay */}
      <div className="absolute inset-0 z-0">
        <img 
          src="https://images.unsplash.com/photo-1519014816548-bf5fe059e98b?auto=format&fit=crop&q=80&w=1920" 
          alt="Avrili Nails Background" 
          className="w-full h-full object-cover"
        />
        <div className="absolute inset-0 bg-white/60 dark:bg-black/70 backdrop-blur-sm"></div>
      </div>

      <div className="relative z-10 container mx-auto px-6 text-center">
        <motion.div
          initial={{ opacity: 0, y: 30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
        >
          <div className="inline-block mb-4 px-4 py-1 rounded-full border border-pink-500 text-pink-600 dark:text-pink-400 font-medium text-sm tracking-widest bg-pink-50 dark:bg-pink-900/20">
            ESTUDIO PROFESIONAL
          </div>
          <h1 className="font-serif text-5xl md:text-7xl lg:text-8xl font-bold text-zinc-900 dark:text-white mb-6">
            Avrili<span className="text-transparent bg-clip-text bg-gradient-to-r from-pink-500 to-purple-500">Nails</span>
          </h1>
          <p className="text-xl md:text-2xl text-zinc-700 dark:text-zinc-300 max-w-2xl mx-auto mb-10 font-light">
            Arte en tus manos. Especialistas en esculpidas, soft gel y diseños personalizados que resaltan tu esencia.
          </p>
          
          <div className="flex flex-col sm:flex-row gap-4 justify-center items-center">
            <button 
              onClick={() => scrollToSection('booking')}
              className="px-8 py-4 bg-zinc-900 dark:bg-white text-white dark:text-black rounded-full font-bold tracking-wide hover:scale-105 transition-transform shadow-lg hover:shadow-pink-500/25 flex items-center gap-2"
            >
              RESERVAR TURNO <Calendar size={18} />
            </button>
            <button 
              onClick={() => scrollToSection('services')}
              className="px-8 py-4 bg-transparent border-2 border-zinc-900 dark:border-white text-zinc-900 dark:text-white rounded-full font-bold tracking-wide hover:bg-zinc-900 hover:text-white dark:hover:bg-white dark:hover:text-black transition-all"
            >
              VER SERVICIOS
            </button>
          </div>
        </motion.div>
      </div>

      <div className="absolute bottom-10 left-1/2 -translate-x-1/2 animate-bounce text-zinc-500 dark:text-zinc-400">
        <span className="text-xs tracking-widest uppercase mb-2 block text-center">Desliza</span>
        <div className="w-0.5 h-12 bg-gradient-to-b from-pink-500 to-transparent mx-auto"></div>
      </div>
    </section>
  );
};

// 3. Services Section
const Services = () => {
  return (
    <section id="services" className="py-24 bg-zinc-50 dark:bg-zinc-900">
      <div className="container mx-auto px-6">
        <div className="text-center mb-16">
          <h2 className="font-serif text-4xl md:text-5xl font-bold text-zinc-900 dark:text-white mb-4">
            Nuestros Servicios
          </h2>
          <div className="w-24 h-1 bg-pink-500 mx-auto rounded-full mb-6"></div>
          <p className="text-zinc-600 dark:text-zinc-400 max-w-2xl mx-auto">
            Utilizamos productos de primera calidad para garantizar la salud de tus uñas y un acabado duradero.
          </p>
        </div>

        <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
          {SERVICES.map((service) => (
            <motion.div 
              key={service.id}
              initial={{ opacity: 0, y: 20 }}
              whileInView={{ opacity: 1, y: 0 }}
              viewport={{ once: true }}
              className="group bg-white dark:bg-zinc-800 rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition-all duration-300 border border-zinc-100 dark:border-zinc-700"
            >
              <div className="flex flex-col md:flex-row h-full">
                <div className="md:w-2/5 h-64 md:h-auto overflow-hidden relative">
                  <img 
                    src={service.img} 
                    alt={service.title} 
                    className="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110"
                  />
                  <div className="absolute top-4 left-4 bg-white/90 dark:bg-black/80 backdrop-blur px-3 py-1 rounded-full text-xs font-bold uppercase tracking-wider text-pink-600 dark:text-pink-400">
                    {service.time}
                  </div>
                </div>
                <div className="md:w-3/5 p-8 flex flex-col justify-between">
                  <div>
                    <div className="flex justify-between items-start mb-4">
                      <h3 className="font-serif text-2xl font-bold text-zinc-900 dark:text-white">{service.title}</h3>
                      <span className="text-xl font-bold text-pink-500">{service.price}</span>
                    </div>
                    <p className="text-zinc-600 dark:text-zinc-300 text-sm mb-4 leading-relaxed">
                      {service.desc}
                    </p>
                    <div className="mb-4">
                      <h4 className="text-xs font-bold uppercase text-zinc-400 mb-2">Incluye:</h4>
                      <p className="text-xs text-zinc-500 dark:text-zinc-400 italic bg-zinc-50 dark:bg-zinc-900/50 p-3 rounded-lg border border-zinc-100 dark:border-zinc-700">
                        {service.includes}
                      </p>
                    </div>
                  </div>
                  <div>
                    <h4 className="text-xs font-bold uppercase text-zinc-400 mb-2">Beneficios:</h4>
                    <ul className="space-y-1">
                      {service.benefits.map((benefit, idx) => (
                        <li key={idx} className="flex items-center gap-2 text-sm text-zinc-600 dark:text-zinc-300">
                          <CheckCircle size={14} className="text-green-500" /> {benefit}
                        </li>
                      ))}
                    </ul>
                  </div>
                </div>
              </div>
            </motion.div>
          ))}
        </div>
      </div>
    </section>
  );
};

// 4. Shop Section
const Shop = ({ addToCart }) => {
  return (
    <section id="shop" className="py-24 bg-white dark:bg-black relative">
      <div className="container mx-auto px-6">
        <div className="flex flex-col md:flex-row justify-between items-end mb-12 gap-4">
          <div>
            <h2 className="font-serif text-4xl md:text-5xl font-bold text-zinc-900 dark:text-white mb-2">
              Avrili Shop <span className="text-pink-500 text-6xl">.</span>
            </h2>
            <p className="text-zinc-500 dark:text-zinc-400">Llevate la experiencia a casa. Press-On nails y cuidados.</p>
          </div>
          <button className="text-pink-500 font-bold hover:text-pink-600 flex items-center gap-2 group">
            Ver todo el catálogo <ChevronRight size={20} className="group-hover:translate-x-1 transition-transform" />
          </button>
        </div>

        <div className="grid grid-cols-2 md:grid-cols-4 gap-6">
          {PRODUCTS.map((product) => (
            <div key={product.id} className="group cursor-pointer">
              <div className="relative overflow-hidden rounded-xl mb-4 aspect-square bg-zinc-100 dark:bg-zinc-800">
                <img 
                  src={product.img} 
                  alt={product.name} 
                  className="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110"
                />
                <button 
                  onClick={() => addToCart(product)}
                  className="absolute bottom-4 right-4 bg-white dark:bg-black text-black dark:text-white p-3 rounded-full shadow-lg translate-y-20 opacity-0 group-hover:translate-y-0 group-hover:opacity-100 transition-all duration-300 hover:bg-pink-500 hover:text-white"
                >
                  <Plus size={20} />
                </button>
                <div className="absolute top-4 left-4 bg-black/70 text-white text-[10px] px-2 py-1 rounded font-bold uppercase">
                  {product.category}
                </div>
              </div>
              <h3 className="font-bold text-zinc-900 dark:text-white group-hover:text-pink-500 transition-colors">{product.name}</h3>
              <p className="text-zinc-500 dark:text-zinc-400">${product.price.toLocaleString()}</p>
            </div>
          ))}
        </div>
        
        {/* Fake Stock Banner based on IG image */}
        <div className="mt-16 bg-pink-100 dark:bg-pink-900/20 rounded-2xl p-8 flex flex-col md:flex-row items-center gap-8 border border-pink-200 dark:border-pink-800">
           <div className="flex-1">
              <h3 className="text-2xl font-serif font-bold text-pink-800 dark:text-pink-300 mb-2">Stock Disponible: Press-On Nails</h3>
              <p className="text-pink-700 dark:text-pink-400 mb-4">
                 ¿No tenés tiempo para un turno? Llevate nuestros sets listos para usar ("Stock Disp" ✨). 
                 Diseños únicos, entrega inmediata.
              </p>
              <button className="bg-pink-500 text-white px-6 py-2 rounded-full font-bold hover:bg-pink-600 transition-colors">
                 Ver Disponibles
              </button>
           </div>
           <div className="w-full md:w-1/3 flex gap-2 overflow-hidden opacity-80">
              <div className="w-1/3 aspect-[3/4] bg-white dark:bg-zinc-800 rounded-lg shadow-sm rotate-[-6deg]"></div>
              <div className="w-1/3 aspect-[3/4] bg-white dark:bg-zinc-800 rounded-lg shadow-sm mt-4"></div>
              <div className="w-1/3 aspect-[3/4] bg-white dark:bg-zinc-800 rounded-lg shadow-sm rotate-[6deg]"></div>
           </div>
        </div>
      </div>
    </section>
  );
};

// 5. Gallery & Testimonials
const GalleryAndReviews = () => {
  return (
    <section id="gallery" className="py-24 bg-zinc-900 text-white overflow-hidden">
      <div className="container mx-auto px-6 mb-16">
        <h2 className="font-serif text-4xl text-center font-bold mb-12">
          Antes & Después <span className="text-pink-500">/</span> Clientes Felices
        </h2>
        
        {/* Infinite Scroll-ish Gallery Grid */}
        <div className="grid grid-cols-2 md:grid-cols-4 gap-4 mb-20">
            <div className="space-y-4 translate-y-8">
                <img src="https://images.unsplash.com/photo-1604654894610-df63bc536371?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
                <img src="https://images.unsplash.com/photo-1519014816548-bf5fe059e98b?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
            </div>
            <div className="space-y-4">
                <img src="https://images.unsplash.com/photo-1632922267756-9b71242b1592?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
                <img src="https://images.unsplash.com/photo-1596462502278-27bfdd403ea2?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
            </div>
             <div className="space-y-4 translate-y-12">
                <img src="https://images.unsplash.com/photo-1522337660859-02fbefca4702?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
                <img src="https://images.unsplash.com/photo-1599693988002-3932e675034c?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
            </div>
            <div className="space-y-4 md:block hidden">
                <img src="https://images.unsplash.com/photo-1620916566398-39f1143ab7be?w=400&q=80" className="rounded-lg hover:opacity-80 transition-opacity" alt="Nail Art" />
                <div className="bg-pink-500 rounded-lg p-6 flex items-center justify-center text-center h-48">
                    <p className="font-serif text-2xl font-bold">Más de 500 sets realizados</p>
                </div>
            </div>
        </div>

        {/* Testimonials */}
        <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            {REVIEWS.map((review) => (
                <div key={review.id} className="bg-zinc-800 p-8 rounded-2xl relative border border-zinc-700">
                    <div className="absolute -top-4 right-8 bg-pink-500 text-white px-3 py-1 rounded-full text-xs font-bold flex gap-1 items-center">
                        {review.rating} <Star size={10} fill="white" />
                    </div>
                    <p className="text-zinc-300 italic mb-6">"{review.text}"</p>
                    <div className="flex items-center gap-4">
                        <img src={review.img} alt={review.name} className="w-10 h-10 rounded-full object-cover" />
                        <h4 className="font-bold text-white">{review.name}</h4>
                    </div>
                </div>
            ))}
        </div>
      </div>
    </section>
  );
};

// 6. Booking Section
const Booking = () => {
  const [formData, setFormData] = useState({
    name: '',
    phone: '',
    email: '',
    service: '',
    date: '',
    time: '',
    notes: ''
  });
  const [status, setStatus] = useState('idle'); // idle, loading, success

  const handleChange = (e) => {
    setFormData({ ...formData, [e.target.name]: e.target.value });
  };

  const handleSubmit = (e) => {
    e.preventDefault();
    setStatus('loading');
    
    // Simulate API call and LocalStorage save
    setTimeout(() => {
        const bookings = JSON.parse(localStorage.getItem('avrili_bookings') || '[]');
        bookings.push({ ...formData, id: Date.now() });
        localStorage.setItem('avrili_bookings', JSON.stringify(bookings));
        
        setStatus('success');
        setFormData({ name: '', phone: '', email: '', service: '', date: '', time: '', notes: '' });
    }, 1500);
  };

  return (
    <section id="booking" className="py-24 bg-pink-50 dark:bg-zinc-900/50">
      <div className="container mx-auto px-6 flex flex-col md:flex-row gap-12 items-center">
        
        <div className="md:w-1/2">
            <h2 className="font-serif text-4xl md:text-5xl font-bold text-zinc-900 dark:text-white mb-6">
                Agendá tu Cita
            </h2>
            <p className="text-zinc-600 dark:text-zinc-400 mb-8 text-lg">
                Reservar es súper fácil. Elegí tu servicio, el día que prefieras y listo. Te confirmaremos por WhatsApp.
            </p>
            
            <div className="space-y-6">
                <div className="flex items-center gap-4">
                    <div className="w-12 h-12 bg-white dark:bg-zinc-800 rounded-full flex items-center justify-center text-pink-500 shadow-md">
                        <MapPin size={24} />
                    </div>
                    <div>
                        <h4 className="font-bold text-zinc-900 dark:text-white">Ubicación del Estudio</h4>
                        <p className="text-zinc-500 dark:text-zinc-400">Belgrano, Buenos Aires (Dirección exacta al confirmar)</p>
                    </div>
                </div>
                <div className="flex items-center gap-4">
                    <div className="w-12 h-12 bg-white dark:bg-zinc-800 rounded-full flex items-center justify-center text-pink-500 shadow-md">
                        <ShieldCheck size={24} />
                    </div>
                    <div>
                        <h4 className="font-bold text-zinc-900 dark:text-white">Políticas de Cancelación</h4>
                        <p className="text-zinc-500 dark:text-zinc-400">Avisar con 24hs de antelación. Seña del 50% requerida.</p>
                    </div>
                </div>
            </div>
        </div>

        <div className="md:w-1/2 w-full bg-white dark:bg-zinc-800 p-8 rounded-3xl shadow-xl border border-pink-100 dark:border-pink-900/30">
            {status === 'success' ? (
                <div className="text-center py-12">
                    <div className="w-20 h-20 bg-green-100 dark:bg-green-900/30 rounded-full flex items-center justify-center mx-auto mb-6 text-green-500">
                        <CheckCircle size={40} />
                    </div>
                    <h3 className="text-2xl font-bold text-zinc-900 dark:text-white mb-2">¡Solicitud Enviada!</h3>
                    <p className="text-zinc-500 dark:text-zinc-400">Gracias por elegir Avrili Nails. Te contactaremos pronto para coordinar la seña.</p>
                    <button onClick={() => setStatus('idle')} className="mt-8 text-pink-500 font-bold hover:underline">Nueva reserva</button>
                </div>
            ) : (
                <form onSubmit={handleSubmit} className="space-y-4">
                    <div className="grid grid-cols-2 gap-4">
                        <div>
                            <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Nombre</label>
                            <input required type="text" name="name" value={formData.name} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white" />
                        </div>
                        <div>
                            <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Teléfono</label>
                            <input required type="tel" name="phone" value={formData.phone} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white" />
                        </div>
                    </div>
                    
                    <div>
                        <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Email</label>
                        <input required type="email" name="email" value={formData.email} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white" />
                    </div>

                    <div>
                        <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Servicio</label>
                        <select required name="service" value={formData.service} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white">
                            <option value="">Seleccionar Servicio...</option>
                            {SERVICES.map(s => <option key={s.id} value={s.title}>{s.title}</option>)}
                        </select>
                    </div>

                    <div className="grid grid-cols-2 gap-4">
                        <div>
                            <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Fecha</label>
                            <input required type="date" name="date" value={formData.date} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white" />
                        </div>
                        <div>
                            <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Horario Pref.</label>
                            <input required type="time" name="time" value={formData.time} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white" />
                        </div>
                    </div>

                    <div>
                        <label className="block text-xs font-bold text-zinc-500 dark:text-zinc-400 uppercase mb-1">Notas / Diseño específico</label>
                        <textarea name="notes" rows="3" value={formData.notes} onChange={handleChange} className="w-full bg-zinc-50 dark:bg-zinc-700 border-none rounded-lg p-3 focus:ring-2 focus:ring-pink-500 dark:text-white"></textarea>
                    </div>

                    <button disabled={status === 'loading'} type="submit" className="w-full bg-black dark:bg-pink-600 text-white py-4 rounded-lg font-bold tracking-wide hover:opacity-90 transition-opacity flex justify-center items-center gap-2">
                        {status === 'loading' ? 'Procesando...' : 'CONFIRMAR RESERVA'}
                    </button>
                </form>
            )}
        </div>
      </div>
    </section>
  );
};

// 7. Footer
const Footer = ({ scrollToSection }) => {
  return (
    <footer className="bg-zinc-900 text-white pt-20 pb-10 border-t border-zinc-800">
      <div className="container mx-auto px-6">
        <div className="grid grid-cols-1 md:grid-cols-4 gap-12 mb-16">
          <div className="col-span-1 md:col-span-2">
            <div className="flex items-center gap-2 mb-6">
              <div className="w-8 h-8 bg-pink-500 rounded-full flex items-center justify-center text-white border border-white">
                <Heart size={16} fill="white" />
              </div>
              <span className="font-serif text-2xl font-bold">Avrili<span className="text-pink-500">Nails</span></span>
            </div>
            <p className="text-zinc-400 max-w-sm mb-6">
              Creando arte en pequeñas superficies. Un espacio dedicado al cuidado y embellecimiento de tus manos con la mejor calidad y estilo.
            </p>
            <div className="flex gap-4">
              <a href="#" className="w-10 h-10 rounded-full bg-zinc-800 flex items-center justify-center hover:bg-pink-500 transition-colors"><Instagram size={20} /></a>
              <a href="#" className="w-10 h-10 rounded-full bg-zinc-800 flex items-center justify-center hover:bg-green-500 transition-colors"><Phone size={20} /></a>
              <a href="#" className="w-10 h-10 rounded-full bg-zinc-800 flex items-center justify-center hover:bg-blue-500 transition-colors"><Mail size={20} /></a>
            </div>
          </div>

          <div>
            <h4 className="font-bold text-lg mb-6">Links Rápidos</h4>
            <ul className="space-y-4 text-zinc-400">
              <li><button onClick={() => scrollToSection('services')} className="hover:text-pink-500 transition-colors">Servicios</button></li>
              <li><button onClick={() => scrollToSection('shop')} className="hover:text-pink-500 transition-colors">Tienda Online</button></li>
              <li><button onClick={() => scrollToSection('booking')} className="hover:text-pink-500 transition-colors">Reservar Turno</button></li>
              <li><button onClick={() => scrollToSection('gallery')} className="hover:text-pink-500 transition-colors">Galería</button></li>
            </ul>
          </div>

          <div>
            <h4 className="font-bold text-lg mb-6">Contacto</h4>
            <ul className="space-y-4 text-zinc-400">
              <li className="flex gap-3"><MapPin size={20} className="text-pink-500" /> Belgrano, CABA</li>
              <li className="flex gap-3"><Clock size={20} className="text-pink-500" /> Mar - Sáb: 10:00 - 19:00</li>
              <li className="flex gap-3"><Mail size={20} className="text-pink-500" /> contacto@avrilinails.com</li>
            </ul>
          </div>
        </div>

        <div className="border-t border-zinc-800 pt-8 flex flex-col md:flex-row justify-between items-center text-zinc-500 text-sm">
          <p>&copy; 2024 Avrili Nails - Delfii Vazquez. Todos los derechos reservados.</p>
          <div className="flex gap-6 mt-4 md:mt-0">
            <a href="#" className="hover:text-white">Términos y Condiciones</a>
            <a href="#" className="hover:text-white">Política de Privacidad</a>
          </div>
        </div>
      </div>
    </footer>
  );
};

// 8. About Section
const About = () => {
    return (
        <section id="about" className="py-24 bg-white dark:bg-black overflow-hidden relative">
            <div className="absolute top-0 right-0 w-1/3 h-full bg-pink-50 dark:bg-pink-900/10 -z-0"></div>
            <div className="container mx-auto px-6 relative z-10">
                <div className="flex flex-col md:flex-row items-center gap-12">
                    <div className="md:w-1/2 relative">
                        <div className="relative z-10 rounded-2xl overflow-hidden shadow-2xl border-4 border-white dark:border-zinc-800">
                             <img src="https://images.unsplash.com/photo-1599693988002-3932e675034c?auto=format&fit=crop&q=80&w=800" alt="Delfii Vazquez" className="w-full" />
                        </div>
                        {/* Decorative elements */}
                        <div className="absolute -bottom-6 -left-6 bg-black text-white p-6 rounded-lg shadow-xl hidden md:block">
                            <p className="font-serif font-bold text-2xl">5+</p>
                            <p className="text-xs uppercase tracking-widest">Años de Exp.</p>
                        </div>
                    </div>
                    <div className="md:w-1/2">
                        <h2 className="font-serif text-4xl md:text-5xl font-bold text-zinc-900 dark:text-white mb-6">
                            Hola, soy Delfii <span className="text-pink-500">.</span>
                        </h2>
                        <h3 className="text-lg font-medium text-pink-500 mb-6 uppercase tracking-widest">Founder & Nail Artist</h3>
                        <p className="text-zinc-600 dark:text-zinc-300 leading-relaxed mb-6">
                            Avrili Nails nació de mi pasión por el arte y la estética. Lo que empezó en una pequeña mesa de mi habitación, hoy es un estudio donde cada detalle cuenta. 
                        </p>
                        <p className="text-zinc-600 dark:text-zinc-300 leading-relaxed mb-8">
                            Me especializo en Soft Gel y Nail Art mano alzada. Mi misión no es solo que tengas uñas lindas, sino que disfrutes de una experiencia de cuidado personal donde te sientas cómoda, escuchada y mimada.
                        </p>
                        
                        <div className="grid grid-cols-2 gap-4">
                            <div className="flex items-center gap-3 bg-zinc-50 dark:bg-zinc-800 p-4 rounded-lg">
                                <Sparkles className="text-pink-500" />
                                <span className="font-bold text-sm dark:text-white">Materiales Importados</span>
                            </div>
                            <div className="flex items-center gap-3 bg-zinc-50 dark:bg-zinc-800 p-4 rounded-lg">
                                <ShieldCheck className="text-pink-500" />
                                <span className="font-bold text-sm dark:text-white">Esterilización Hospitalaria</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    )
}

// 9. Shopping Cart Modal
const CartModal = ({ isOpen, onClose, cartItems, updateQuantity, removeFromCart }) => {
    if (!isOpen) return null;

    const total = cartItems.reduce((acc, item) => acc + (item.price * item.quantity), 0);

    return (
        <div className="fixed inset-0 z-[60] flex justify-end">
            <div className="absolute inset-0 bg-black/50 backdrop-blur-sm" onClick={onClose}></div>
            <motion.div 
                initial={{ x: '100%' }}
                animate={{ x: 0 }}
                exit={{ x: '100%' }}
                className="relative w-full max-w-md bg-white dark:bg-zinc-900 h-full shadow-2xl flex flex-col"
            >
                <div className="p-6 flex justify-between items-center border-b dark:border-zinc-800">
                    <h2 className="font-serif text-2xl font-bold dark:text-white">Tu Carrito ({cartItems.length})</h2>
                    <button onClick={onClose} className="p-2 hover:bg-zinc-100 dark:hover:bg-zinc-800 rounded-full dark:text-white">
                        <X size={24} />
                    </button>
                </div>

                <div className="flex-1 overflow-y-auto p-6 space-y-6">
                    {cartItems.length === 0 ? (
                        <div className="flex flex-col items-center justify-center h-full text-zinc-400">
                            <ShoppingBag size={48} className="mb-4 opacity-50" />
                            <p>El carrito está vacío.</p>
                        </div>
                    ) : (
                        cartItems.map(item => (
                            <div key={item.id} className="flex gap-4">
                                <img src={item.img} alt={item.name} className="w-20 h-20 object-cover rounded-lg bg-zinc-100" />
                                <div className="flex-1">
                                    <h4 className="font-bold text-zinc-900 dark:text-white">{item.name}</h4>
                                    <p className="text-pink-500 font-medium">${item.price}</p>
                                    <div className="flex items-center gap-3 mt-2">
                                        <button onClick={() => updateQuantity(item.id, -1)} className="p-1 bg-zinc-100 dark:bg-zinc-800 rounded dark:text-white"><Minus size={14} /></button>
                                        <span className="text-sm font-bold dark:text-white">{item.quantity}</span>
                                        <button onClick={() => updateQuantity(item.id, 1)} className="p-1 bg-zinc-100 dark:bg-zinc-800 rounded dark:text-white"><Plus size={14} /></button>
                                        <button onClick={() => removeFromCart(item.id)} className="ml-auto text-red-400 hover:text-red-500"><Trash2 size={16} /></button>
                                    </div>
                                </div>
                            </div>
                        ))
                    )}
                </div>

                {cartItems.length > 0 && (
                    <div className="p-6 border-t dark:border-zinc-800 bg-zinc-50 dark:bg-zinc-900">
                        <div className="flex justify-between items-center mb-4">
                            <span className="text-zinc-600 dark:text-zinc-400">Total Estimado</span>
                            <span className="text-2xl font-bold text-zinc-900 dark:text-white">${total.toLocaleString()}</span>
                        </div>
                        <button className="w-full bg-black dark:bg-pink-600 text-white py-4 rounded-full font-bold hover:opacity-90 transition-opacity">
                            INICIAR COMPRA
                        </button>
                    </div>
                )}
            </motion.div>
        </div>
    );
};

// --- MAIN APP ---

function App() {
  const [darkMode, setDarkMode] = useState(false);
  const [cartOpen, setCartOpen] = useState(false);
  const [cart, setCart] = useState([]);

  // Load cart from local storage on mount
  useEffect(() => {
    const savedCart = localStorage.getItem('avrili_cart');
    if (savedCart) setCart(JSON.parse(savedCart));
    
    // Check system preference for dark mode
    if (window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches) {
        setDarkMode(true);
    }
  }, []);

  // Save cart to local storage whenever it changes
  useEffect(() => {
    localStorage.setItem('avrili_cart', JSON.stringify(cart));
  }, [cart]);

  const toggleTheme = () => setDarkMode(!darkMode);

  const scrollToSection = (id) => {
    const element = document.getElementById(id);
    if (element) {
      element.scrollIntoView({ behavior: 'smooth' });
    }
  };

  const addToCart = (product) => {
    setCart(prev => {
        const existing = prev.find(item => item.id === product.id);
        if (existing) {
            return prev.map(item => item.id === product.id ? { ...item, quantity: item.quantity + 1 } : item);
        }
        return [...prev, { ...product, quantity: 1 }];
    });
    setCartOpen(true);
  };

  const updateQuantity = (id, delta) => {
      setCart(prev => prev.map(item => {
          if (item.id === id) {
              const newQty = Math.max(1, item.quantity + delta);
              return { ...item, quantity: newQty };
          }
          return item;
      }));
  };

  const removeFromCart = (id) => {
      setCart(prev => prev.filter(item => item.id !== id));
  };

  return (
    <div className={`${darkMode ? 'dark' : ''}`}>
      <div className="bg-white dark:bg-black min-h-screen transition-colors duration-300 font-sans selection:bg-pink-200 dark:selection:bg-pink-900">
        
        <Navbar 
            cartCount={cart.reduce((a, b) => a + b.quantity, 0)} 
            toggleCart={() => setCartOpen(true)} 
            darkMode={darkMode} 
            toggleTheme={toggleTheme}
            scrollToSection={scrollToSection}
        />
        
        <CartModal 
            isOpen={cartOpen} 
            onClose={() => setCartOpen(false)} 
            cartItems={cart}
            updateQuantity={updateQuantity}
            removeFromCart={removeFromCart}
        />

        <main>
            <Hero scrollToSection={scrollToSection} />
            <About />
            <Services />
            <Shop addToCart={addToCart} />
            <GalleryAndReviews />
            <Booking />
        </main>

        <Footer scrollToSection={scrollToSection} />

        {/* WhatsApp Float */}
        <a 
            href="https://wa.me/" 
            target="_blank" 
            rel="noopener noreferrer"
            className="fixed bottom-6 right-6 z-40 bg-green-500 text-white p-4 rounded-full shadow-lg hover:scale-110 transition-transform hover:shadow-green-500/30 flex items-center justify-center"
        >
            <Phone size={24} fill="currentColor" />
        </a>
      </div>
    </div>
  );
}

export default App;