# Laravel + React JSX + DaisyUI Starter Kit

🚀 **Introduction**

This is a DaisyUI-powered version of the Laravel React JSX Starter Kit.  
It provides a modern and elegant setup for building Laravel applications with a React frontend using Inertia, TailwindCSS 4, and DaisyUI.

Unlike the TypeScript-based versions, this kit uses **pure JavaScript (.jsx)**, making it perfect for developers who prefer simplicity and speed over TypeScript complexity.

It comes preconfigured with Laravel 12, React 19, Inertia 2, TailwindCSS 4, and DaisyUI — giving you everything you need to build beautiful, responsive, and modern web applications.

---

## 🎯 Features

✅ **React 19 + JSX** – No TypeScript, just JavaScript  
✅ **Laravel 12** – The latest version of Laravel for a powerful backend  
✅ **Inertia 2** – Seamless single-page app experience  
✅ **TailwindCSS 4 + DaisyUI** – Fast and elegant UI styling  
✅ **Vite** – Super-fast development with hot module replacement  
✅ **Testing Support** – PHPUnit & Pest preinstalled  
✅ **Zero Configuration Required** – Just install and start coding!

---

## 🛠 Installation

### 1️⃣ Create a new Laravel app using the starter kit

```bash
laravel new --using=Szyron/react-jsx-daisyui-starter-kit react-daisyui-app
```
### 2️⃣ Install Dependencies
```bash
cd react-daisyui-app
composer install
npm install
```

### 3️⃣ Setup Environment
Copy the `.env.example` environment file and generate your application key:

```bash
cp .env.example .env
php artisan key:generate
```

### 4️⃣ Run Database Migrations
```bash
php artisan migrate --seed
```

### 5️⃣ Install DaisyUI
DaisyUI is a TailwindCSS plugin that adds a beautiful component library to your project. 
```bash
npm install tailwindcss@latest @tailwindcss/vite@latest daisyui@latest
```
More info about [DaisyUI](https://daisyui.com/docs/install/vite/)

### 6️⃣ Import DaisyUI

To enable DaisyUI components in your project, you need to import the plugin in your main CSS file.  

Open `resources/css/app.css` and add the following:

```css
/* resources/css/app.css */

/* Tailwind base styles */
@tailwind base;
@tailwind components;
@tailwind utilities;

/* DaisyUI plugin */
@plugin "daisyui";
```

### 7️⃣ Start the Development Environment
```bash
composer dev
```
Your app is now running! 🎉

---

### 🎨 DaisyUI Integration
This starter kit includes DaisyUI, a powerful TailwindCSS plugin that provides a wide range of prebuilt, customizable UI components.

You can easily use DaisyUI components throughout your React JSX pages and components.

Example:

```bash
export default function Example() {
  return (
    <div className="p-4">
      <button className="btn btn-primary">Hello DaisyUI!</button>
    </div>
  );
}
```
---
### 📚 Official Documentation
You can find the official documentation for:

Documentation for all Laravel starter kits can be found on the [Laravel website]((https://laravel.com/docs/12.x/contributions).
Get started with daisyUI and explore its full documentation at [DaisyUI website](https://daisyui.com/docs/intro/)

---

### 🤝 Contributing
Thank you for considering contributing to this starter kit!
Please refer to the Laravel contribution guide for best practices.

---

### 📜 Code of Conduct
Please review and abide by the Laravel Code of Conduct to ensure our community remains welcoming to everyone.

---

### ⚖️ License
The Laravel + React JSX + DaisyUI Starter Kit is open-sourced software licensed under the MIT license.

---

### 👏 Credits
Original Laravel React JSX Starter Kit by [Yazid KHALDI](https://github.com/YazidKHALDI)

DaisyUI Integration and Enhancement by [Szyron](https://github.com/Szyron)

---
Happy coding! 🚀
