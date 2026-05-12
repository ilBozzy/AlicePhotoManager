# Alice

### A High-Performance Desktop Photo Manager

**Alice** is a standalone photo gallery engine engineered for speed. It is specifically built to handle massive archives consisting of hundreds of gigabytes and tens of thousands of files while avoiding the performance degradation typical of standard image viewers.

The core philosophy of Alice is the maintenance of **Flow**. The primary objective is to eliminate "presura"—the unnecessary mental stress caused by infinite loading times—allowing the user to navigate through memories in a fluid, natural, and uninterrupted manner.

---

## ⚠️ Disclaimer and Limitation of Liability

Before proceeding with this software, you must read and understand the following conditions. This binary does not possess a certified digital signature. Windows Defender or other antivirus software will likely flag it as a potential threat, which is expected behavior for unsigned software in development. The developer assumes no responsibility or liability for any direct or indirect damage to hardware or software, data loss, or system instability. Use of this software is strictly at your own risk. This is a Beta version intended exclusively for advanced users who understand the risks of executing testing-phase code. The software is portable and requires no installation; simply extract the archive and run the executable.

---

## 🚀 Features

Alice is optimized for speed and capable of managing 300GB+ libraries with immediate response times. It utilizes advanced Virtual Scrolling and Lazy Loading where images are rendered via GPU only when necessary and resources are freed as soon as they leave the screen. A parallel multi-threaded indexer analyzes files and EXIF metadata without blocking the interface. Thumbnails are generated on-the-fly and managed through a dynamic Least Recently Used (LRU) cache to ensure smooth navigation. The frameless interface offers a modern design with native Windows API integration for seamless window dragging and system controls.

---

## 🛠️ Tech Stack and Development

The software leverages a hybrid architecture for stability and flexibility. The backend is powered by Python 3 for system logic and I/O while the database utilizes SQLite3 with Write-Ahead Logging (WAL) for rapid transactions. The frontend is built with Vanilla JavaScript, HTML5, and CSS3 to ensure maximum efficiency without framework overhead. Iconography is provided by Lucide Icons under the free ISC license. The optimization and debugging process was supported by Claude (Anthropic) to ensure clean code structure and efficient thread management.

---

## ⚖️ Legal Notes and Distribution

Alice is developed for personal and educational utility and has no commercial purpose. It is strictly prohibited to sell, monetize, or commercialize this software in any form. The software may not be redistributed or republished on other portals without explicit authorization and is intended for individual use only.

---

## 🤝 Contributing

Pull Requests are welcome, particularly those focused on further loading optimizations. The fundamental rule for all contributions is that the main UI thread must remain entirely free to guarantee the Flow.
