function Home() {
  return (
    <div className="min-h-screen bg-gray-50 text-gray-900 flex flex-col items-center justify-center p-6">
      <header className="w-full max-w-4xl text-center mb-12">
        <h1 className="text-4xl font-extrabold text-gray-800">Portfólio Rafaela Ribeiro</h1>
        <p className="text-lg text-gray-600 mt-2">Redação Jornalística | SEO | Assessoria de Imprensa</p>
      </header>
      
      <main className="w-full max-w-4xl">
        <section className="mb-12">
          <h2 className="text-2xl font-semibold text-gray-800">Sobre Mim</h2>
          <p className="text-gray-700 mt-4">
            Sou jornalista apaixonada por contar histórias e compartilhar informações de maneira clara e envolvente, com foco em resultados e SEO.
          </p>
        </section>
        
        <section className="mb-12">
          <h2 className="text-2xl font-semibold text-gray-800">Portfólio</h2>
          <ul className="list-disc pl-6 mt-4 space-y-2">
            <li><a href="#" className="text-blue-600 hover:underline">Título do Artigo 1</a></li>
            <li><a href="#" className="text-blue-600 hover:underline">Título do Artigo 2</a></li>
            <li><a href="#" className="text-blue-600 hover:underline">Título do Artigo 3</a></li>
          </ul>
        </section>
        
        <section>
          <h2 className="text-2xl font-semibold text-gray-800">Contato</h2>
          <p className="text-gray-700 mt-4">
            Entre em contato comigo através do e-mail: 
            <a href="mailto:email@exemplo.com" className="text-blue-600 hover:underline ml-1">email@exemplo.com</a>
          </p>
        </section>
      </main>
    </div>
  );
}

export default Home;
