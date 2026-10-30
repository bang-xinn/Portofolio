# AGENTS.md

## Project

Single-file static portfolio at `index.html`. No build step, package manager, tests, or linter. Open the file directly in a browser (or serve it through Laragon at `C:\laragon\www\portofolio`).

- Styling uses Tailwind CSS **Play CDN** plus a small inline `<style>` block. There is no Tailwind config file; theme customizations live in the inline `tailwind.config` script.
- Fonts load from Google Fonts (Inter). The page needs internet access for Tailwind and fonts.
- Content is in Indonesian. Keep copy in Indonesian unless asked otherwise.
- Sections are anchored by `#beranda`, `#tentang`, `#keahlian`, `#pengalaman`, `#proyek`, `#sertifikasi`, `#kontak`; keep these IDs when editing navigation.

## Assets

| Used in HTML | Source / notes |
| --- | --- |
| `assets/images/foto-profil.jpg` | Web-optimized 1000×1333 JPG generated from `assets/images/foto_profile.heic` (original kept as source). Re-export if the photo changes. |
| `assets/images/logo-unp.png` | UNP logo, transparent PNG. |
| `assets/images/logo-kemenkumham.png` | Kemenkumham logo, transparent PNG. |
| `assets/images/sma_dian.jpg` | SMA Dian Andalas Padang logo, shown on the Guru Magang card. |
| `assets/images/logo_kkn.jpeg` | KKN Nagari Sasak logo, shown on the Ketua KKN card. |
| `assets/images/logo-kasirq.png` | Original KasirQ logo with large off-white margins (source file, not used directly in HTML). |
| `assets/images/logo-kasirq-mark.png` | Trimmed 700×269 KasirQ logo used in the project card. |
| `assets/images/logo-sinta-5.jpg` | Sinta 5 journal logo, shown on the publication card. |
| `assets/images/buruh.png` | Poster design thumbnail in the "Desain Visual & Konten" card. |
| `assets/images/kartini.png` | Poster design thumbnail in the "Desain Visual & Konten" card. |
| `assets/images/kebangkitan.png` | Poster design thumbnail in the "Desain Visual & Konten" card. |
| `assets/certificates/ai-fluency-anthropic.pdf` | Anthropic AI Fluency certificate. |
| `assets/certificates/emotional-intelligence-gnik-kemnaker.pdf` | GNIK & Kemnaker Emotional Intelligence certificate (score 95). |
| `assets/certificates/english-proficiency-lpt-unp.pdf` | **Not present.** The LPT UNP card currently links to a `mailto:` request instead of a download. If the PDF is added, replace that link with a `download` link to this path. |

Images use `onerror` to hide themselves when missing, so a missing asset may fail silently. When renaming a file, update the HTML reference too.

## External links

- GitHub profile: `https://github.com/bang-xinn`
- KasirQ repository: `https://github.com/bang-xinn/kasirq`
- Publication DOI: `https://doi.org/10.31004/joecy.v6i2.13944`

## Notes

- Tailwind Play CDN is intended for development/prototyping. For production, compile Tailwind and remove the CDN script instead of relying on it.
- There is no automated verification. After edits, open the page in a browser and check the mobile menu, reveal animations, and asset links.
