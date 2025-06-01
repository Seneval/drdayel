Installation & Project Types:

Next.js / React projects: Ensure the lucide-react package is installed by running npm install lucide-react

Plain HTML/CSS/JS projects: Include Lucide via CDN by adding a script tag pointing to https://unpkg.com/lucide@latest/dist/umd/lucide.js and then calling lucide.createIcons() once in your markup


Never hand-code or output raw <svg> for standard icons

Next.js / React: always import icons from lucide-react (e.g. import { CheckCircle, X } from 'lucide-react') and use them as JSX components (e.g. <CheckCircle size={24} />)

HTML/CSS/JS: always insert icons via the Lucide global API, e.g. <i data-lucide="coffee" data-size="24"></i> and then invoke lucide.createIcons()

Behavior:

Import or include:

React: import desired icons at the top of your file (import { Coffee } from 'lucide-react')

HTML/CSS/JS: place <script src="https://unpkg.com/lucide@latest/dist/umd/lucide.js"></script> in your page and call lucide.createIcons()

Use as components or data elements:

React: render <Coffee size={24} /> where the icon is needed

HTML/CSS/JS: add <i data-lucide="coffee" data-size="24"></i> in your HTML

No inline SVGs: always rely on the Lucide library for consistency and maintainability

Example (React): import { Coffee } from 'lucide-react', then use <Coffee size={24} />
Example (HTML/CSS/JS): include the CDN script, then <i data-lucide="coffee" data-size="24"></i> and execute lucide.createIcons()
