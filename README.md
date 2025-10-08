# Ex09 Event Registration Web Application
## Date:

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
import React from "react";
import img11 from "./img-1-1.png";
import img21 from "./img-2-1.png";

export const IphonePro = (): JSX.Element => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[411px] min-h-[874px] relative">
      <img
        className="absolute top-0 left-0 w-[411px] h-[874px] aspect-[0.54] object-cover"
        alt="Hostel Fest background with colorful powder explosion"
        src={img11}
      />

      <div className="absolute top-[72px] left-[-485px] w-[402px] h-[874px] bg-white overflow-hidden">
        <img
          className="absolute top-[-341px] left-[-217px] w-[715px] h-[1077px] aspect-[0.66] object-cover"
          alt="Secondary background image"
          src={img21}
        />

        <div className="absolute top-[110px] left-[54px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-5xl tracking-[0] leading-[normal]">
          Hostel&nbsp;&nbsp;Fest
        </div>
      </div>

      <header className="absolute top-20 left-[88px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-5xl tracking-[0] leading-[normal]">
        Hostel Fest
      </header>

      <button
        className="absolute top-[464px] left-[97px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-5xl tracking-[0] leading-[normal] cursor-pointer hover:opacity-90 transition-opacity"
        type="button"
        aria-label="Register for Hostel Fest"
      >
        REGISTER
      </button>
    </div>
  );
};
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
frame2
import React from "react";
import imag41 from "./imag-4-1.png";

export const IphonePro = (): JSX.Element => {
  const events = [
    "Cook without fire",
    "DJ",
    "Ramp walk",
    "Solo singing",
    "Group dance",
  ];

  return (
    <div className="bg-white w-full min-w-[402px] min-h-[874px] relative">
      <img
        className="absolute top-0 left-0 w-[402px] h-[874px] aspect-[0.61] object-cover"
        alt="Colorful abstract background with vibrant clouds"
        src={imag41}
      />

      <header className="absolute top-[92px] left-6">
        <h1 className="[font-family:'Inter-Bold',Helvetica] font-bold text-[#f31621] text-[40px] tracking-[0] leading-[normal] whitespace-nowrap">
          Hostel Fest Events
        </h1>
      </header>

      <main className="absolute top-[215px] left-[94px]">
        <ul
          className="[font-family:'Inter-Bold',Helvetica] font-bold text-[#141212] text-[40px] tracking-[0] leading-[normal] list-none"
          role="list"
          aria-label="Event list"
        >
          {events.map((event, index) => (
            <li key={index} className="mb-0">
              *{event}
            </li>
          ))}
        </ul>
      </main>
    </div>
  );
};
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
frame3
import React, { useState } from "react";
import images31 from "./images-3-1.png";

export const IphonePro = (): JSX.Element => {
  const [formData, setFormData] = useState({
    name: "",
    email: "",
    gender: "",
    phone: "",
    department: "",
  });

  const handleInputChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLSelectElement>,
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({
      ...prev,
      [name]: value,
    }));
  };

  const handleSubmit = (e: React.FormEvent<HTMLFormElement>) => {
    e.preventDefault();
    console.log("Form submitted:", formData);
  };

  return (
    <div className="bg-white w-full min-w-[402px] min-h-[861px] relative">
      <img
        className="absolute top-0 left-0 w-[402px] h-[861px] aspect-[0.55] object-cover"
        alt="Background gradient"
        src={images31}
      />

      <form onSubmit={handleSubmit} className="relative z-10">
        <div className="absolute top-[74px] left-[41px] w-[320px]">
          <label
            htmlFor="name"
            className="block [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal] mb-2"
          >
            NAME:
          </label>
          <input
            type="text"
            id="name"
            name="name"
            value={formData.name}
            onChange={handleInputChange}
            className="w-full bg-white bg-opacity-20 border-b-2 border-white text-white text-[24px] px-2 py-1 mb-6 placeholder-white placeholder-opacity-60 focus:bg-opacity-30 focus:outline-none transition-all"
            placeholder="Enter your name"
            required
            aria-label="Name"
          />

          <label
            htmlFor="email"
            className="block [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal] mb-2"
          >
            EMAIL ADDRESS:
          </label>
          <input
            type="email"
            id="email"
            name="email"
            value={formData.email}
            onChange={handleInputChange}
            className="w-full bg-white bg-opacity-20 border-b-2 border-white text-white text-[24px] px-2 py-1 mb-6 placeholder-white placeholder-opacity-60 focus:bg-opacity-30 focus:outline-none transition-all"
            placeholder="Enter your email"
            required
            aria-label="Email Address"
          />

          <label
            htmlFor="gender"
            className="block [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal] mb-2"
          >
            GENDER:
          </label>
          <select
            id="gender"
            name="gender"
            value={formData.gender}
            onChange={handleInputChange}
            className="w-full bg-white bg-opacity-20 border-b-2 border-white text-white text-[24px] px-2 py-1 mb-6 focus:bg-opacity-30 focus:outline-none transition-all"
            required
            aria-label="Gender"
          >
            <option value="" className="text-gray-800">
              Select gender
            </option>
            <option value="male" className="text-gray-800">
              Male
            </option>
            <option value="female" className="text-gray-800">
              Female
            </option>
            <option value="other" className="text-gray-800">
              Other
            </option>
            <option value="prefer-not-to-say" className="text-gray-800">
              Prefer not to say
            </option>
          </select>

          <label
            htmlFor="phone"
            className="block [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal] mb-2"
          >
            PHONE NUMBER:
          </label>
          <input
            type="tel"
            id="phone"
            name="phone"
            value={formData.phone}
            onChange={handleInputChange}
            className="w-full bg-white bg-opacity-20 border-b-2 border-white text-white text-[24px] px-2 py-1 mb-6 placeholder-white placeholder-opacity-60 focus:bg-opacity-30 focus:outline-none transition-all"
            placeholder="Enter your phone"
            required
            aria-label="Phone Number"
          />

          <label
            htmlFor="department"
            className="block [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal] mb-2"
          >
            DEPARTMENT:
          </label>
          <input
            type="text"
            id="department"
            name="department"
            value={formData.department}
            onChange={handleInputChange}
            className="w-full bg-white bg-opacity-20 border-b-2 border-white text-white text-[24px] px-2 py-1 placeholder-white placeholder-opacity-60 focus:bg-opacity-30 focus:outline-none transition-all"
            placeholder="Enter your department"
            required
            aria-label="Department"
          />
        </div>

        <button
          type="submit"
          className="absolute top-[641px] left-[39px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal] cursor-pointer hover:opacity-80 transition-opacity focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-transparent px-4 py-2"
          aria-label="Submit registration form"
        >
          FILL THE REGISTER
          <br />
          FORM
        </button>
      </form>
    </div>
  );
};
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

frame4
import React from "react";
import img22 from "./img-2-2.png";

export const IphonePro = (): JSX.Element => {
  return (
    <main className="bg-white w-full min-w-[398px] min-h-[844px] relative">
      <img
        className="absolute top-0 left-0 w-[398px] h-[844px] aspect-[0.56] object-cover"
        alt="Colorful abstract background with smoke and vibrant colors"
        src={img22}
      />

      <h1 className="absolute top-[68px] left-12 [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[40px] tracking-[0] leading-[normal]">
        THANK YOU
        <br />
        <br />
        FOR <br />
        <br />
        JOINING
        <br />
        <br />
        WITH US...
      </h1>
    </main>
  );
};
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
```


## OUTPUT:
![alt text](<Screenshot 2025-10-08 202548.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
