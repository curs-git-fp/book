# Generació de material educatiu amb mdBook i reveal.js

---

## Introducció

- **mdBook** és una eina per crear llibres, manuals i apunts a partir de fitxers **Markdown**.
- **reveal.js** és una biblioteca JavaScript per crear **presentacions interactives** en HTML.
- Ambdues eines permeten generar **material educatiu eficient, visual i fàcilment compartible**.
- Avantatges:
  - Format **web interactiu** i navegable.
  - Contingut en **Markdown** (senzill d'escriure).
  - Possibilitat d'**integració amb GitHub Pages** per publicar online.

---

## mdBook

- Creat inicialment per a la documentació de **Rust**.
- Permet escriure un llibre amb Markdown i exportar-lo com a web navegable.
- Característiques:
  - Genera índex i navegació automàtica.
  - Suporta cerca integrada.
  - Suporta temes i estils personalitzats.
  - Es pot desplegar fàcilment amb GitHub Pages.

---

## Instal·lació

1. Assegura't de tenir instal·lat **Rust**: [Instal·lació](https://www.rust-lang.org/tools/install).
2. Executa la següent ordre per instal·lar mdBook:

```sh
cargo install mdbook
```

---

## Estructura bàsica

- `book.toml`: configuració del llibre.
- `src/SUMMARY.md`: índex de continguts.
- `src/*.md`: capítols en Markdown.

---

## Generar i veure el llibre

```sh
mdbook build   # genera el llibre a /book
mdbook serve   # inicia un servidor local (http://localhost:3000)
```

---

## reveal.js

- Biblioteca de presentacions en HTML5.
- Es poden crear diapositives amb Markdown o HTML.
- Funcionalitats destacades:
  - Navegació amb teclat o gestos.
  - Fragments (mostrar elements pas a pas).
  - Temes i estils personalitzats.
  - Possibilitat d'afegir vídeos, codis, gràfics...

---

## Com executar

### 1. Instal·lar reveal.js

Pots obtenir reveal.js de dues maneres:

- **Clonar el repositori oficial**:

```sh
git clone https://github.com/hakimel/reveal.js.git
cd reveal.js
````

- **Instal·lar amb npm** (recomanat si ja tens Node.js):

```sh
npm install reveal.js
```

---v

### 2. Llançar el servidor de desenvolupament

Dins la carpeta de reveal.js executa:

```sh
npm start
```

Això obrirà automàticament la presentació al navegador: `http://localhost:8000`

---v

### 3. Crear la teva presentació

- Pots editar el fitxer `index.html` per afegir diapositives en HTML o Markdown.
- Exemple senzill amb Markdown:

```html
<section data-markdown>
<textarea data-template>
# Primera diapositiva

 ---

## Segona diapositiva

- Punt 1
- Punt 2
</textarea>
</section>
```

---v

### 4. Exportar o publicar

- Les presentacions reveal.js són **fitxers HTML estàtics**, així que només cal copiar-los a un servidor web o a **GitHub Pages**.

---

## Integració amb GitHub Pages

- Tant **mdBook** com **reveal.js** poden publicar-se fàcilment amb GitHub Pages:
  1. Crea un repositori GitHub.
  2. Afegeix els fitxers del llibre/presentació.
  3. Activa **Pages** a les opcions del repositori.
  4. Tria la branca i carpeta on es generen els fitxers (`/book`, `/docs`, etc.).
- Exemple:
  - `https://usuari.github.io/projecte/`

---

## Bones pràctiques

- Mantenir els capítols i diapositives en **fitxers separats** per facilitar la lectura.
- Utilitzar **imatges i gràfics** per fer el contingut més visual.
- Afegir **enllaços i recursos addicionals**.
- Si és per a estudiants, combinar **mdBook per apunts i reveal.js per presentacions**.

---

## 🔗 Enllaços

- [mdBook GitHub](https://github.com/rust-lang/mdBook)
- [mdBook Documentation](https://rust-lang.github.io/mdBook/)
- [reveal.js](https://revealjs.com/)
- [Exemples d'ús de reveal.js](https://revealjs.com/demo/)
- [Deploy amb GitHub Pages](https://pages.github.com/)
