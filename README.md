// Site e-commerce moderne pour ONE DIRECT VISION

// Technologies utilisées : React + Tailwind CSS

export default function OneDirectVision() {
  return (
    <main className="bg-gradient-to-br from-gray-900 to-black min-h-screen text-white">
      <header className="p-6 flex justify-between items-center border-b border-gray-700">
        <div className="flex items-center gap-3">
          <img src="/logo.png" alt="1D Vision logo" className="h-12" />
          <h1 className="text-2xl font-bold">ONE DIRECT VISION</h1>
        </div>
        <nav className="flex gap-6 text-sm">
          <a href="#home" className="hover:text-blue-400">Accueil</a>
          <a href="#services" className="hover:text-blue-400">Services</a>
          <a href="#about" className="hover:text-blue-400">À propos</a>
          <a href="#contact" className="hover:text-blue-400">Contact</a>
          <a href="#cart" className="hover:text-blue-400">Panier</a>
        </nav>
      </header>

      {/* Page Accueil */}
      <section id="home" className="py-20 text-center">
        <h2 className="text-4xl font-bold mb-4">Bienvenue chez ONE DIRECT VISION</h2>
        <p className="text-lg text-gray-300 max-w-2xl mx-auto">
          Votre solution sur mesure pour booster votre business : design, marketing, e-commerce, impression, digital & plus !
        </p>
      </section>

      {/* Page Services */}
      <section id="services" className="py-16 px-4">
        <h3 className="text-3xl font-semibold mb-10 text-center">Nos Services</h3>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
          <ServiceCard title="Identité Visuelle" desc="Logo, charte graphique, branding complet" />
          <ServiceCard title="Marketing Digital" desc="Campagnes, gestion réseaux sociaux, contenu" />
          <ServiceCard title="Développement Web" desc="Sites vitrines, e-commerce, sur mesure" />
          <ServiceCard title="Impression 3D / Flyers" desc="Supports physiques personnalisés" />
          <ServiceCard title="E-commerce" desc="Création boutique + système de commande/livraison" />
          <ServiceCard title="Publicité" desc="Campagnes digitales & physiques partout en Algérie" />
        </div>
      </section>

      {/* Page À propos */}
      <section id="about" className="py-16 px-4 bg-gray-800">
        <h3 className="text-3xl font-semibold mb-6 text-center">À propos de 1D Vision</h3>
        <p className="max-w-3xl mx-auto text-gray-300 text-center">
          1D Vision, basée à Saoula, est bien plus qu’une agence. C’est une équipe passionnée au service des marques, entreprises & influenceurs. Notre mission ? Accompagner vos projets avec stratégie, créativité & performance.
        </p>
      </section>

      {/* Page Contact */}
      <section id="contact" className="py-16 px-4">
        <h3 className="text-3xl font-semibold mb-8 text-center">Contactez-nous</h3>
        <form className="max-w-xl mx-auto grid gap-4">
          <input type="text" placeholder="Nom" className="p-3 rounded bg-gray-900 border border-gray-600" />
          <input type="email" placeholder="Email" className="p-3 rounded bg-gray-900 border border-gray-600" />
          <textarea placeholder="Message" className="p-3 rounded bg-gray-900 border border-gray-600"></textarea>
          <button className="bg-blue-600 py-3 rounded hover:bg-blue-500">Envoyer</button>
        </form>
      </section>

      {/* Page Panier */}
      <section id="cart" className="py-16 px-4 bg-gray-900">
        <h3 className="text-3xl font-semibold mb-6 text-center">Mon Panier</h3>
        <p className="text-center text-gray-400">Votre panier est vide pour le moment.</p>
        {/* Système de panier + commande + livraison à intégrer plus tard */}
      </section>

      <footer className="text-center py-6 border-t border-gray-700 text-sm text-gray-500">
        <div className="flex justify-center gap-4 mb-2">
          <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" className="hover:text-white">Facebook</a>
          <a href="https://instagram.com" target="_blank" rel="noopener noreferrer" className="hover:text-white">Instagram</a>
          <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" className="hover:text-white">LinkedIn</a>
        </div>
        © 2025 ONE DIRECT VISION. Tous droits réservés.
      </footer>
    </main>
  );
}

function ServiceCard({ title, desc }) {
  return (
    <div className="bg-gray-800 p-6 rounded-2xl shadow-md hover:shadow-xl transition">
      <h4 className="text-xl font-bold mb-2 text-blue-400">{title}</h4>
      <p className="text-gray-300">{desc}</p>
    </div>
  );
}
