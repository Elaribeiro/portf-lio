function Home() {
  return (
    <div className="min-h-screen bg-gray-100 text-gray-900 flex flex-col items-center justify-center p-6">
      <header className="w-full max-w-4xl text-center mb-10">
        <h1 className="text-4xl font-bold">Meu Portfólio</h1>
        <p className="text-lg text-gray-600">Redação Jornalística |SEO| Assessoria de Imprensa </p>
      </header>
      
      <main className="w-full max-w-4xl">
        <section className="mb-10">
          <h2 className="text-2xl font-semibold">Sobre Mim</h2>
          <p className="text-gray-700 mt-2">
            Sou um(a) jornalista apaixonado(a) por contar histórias e compartilhar informações de forma clara e envolvente.
          </p>
        </section>
        
        <section className="mb-10">
          <h2 className="text-2xl font-semibold">Portfólio Rafaela Ribeiro</h2>
          <ul className="list-disc pl-5 mt-2">
            <li><a href="#" className="text-blue-500 hover:underline">Título do Artigo 1</a></li>
            <li><a href="#" className="text-blue-500 hover:underline">Título do Artigo 2</a></li>
            <li><a href="#" className="text-blue-500 hover:underline">Título do Artigo 3</a></li>
          </ul>
        </section>
        
        <section>
          <h2 className="text-2xl font-semibold">Contato</h2>
          <p className="text-gray-700 mt-2">Entre em contato comigo através do e-mail: <a href="mailto:email@exemplo.com" className="text-blue-500 hover:underline">email@exemplo.com</a></p>
        </section>
      </main>
    </div>
  );
}

export default Home;


