# Ex09 Event Registration Web Application
## Date:08-10-2025

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
~~~
Frame 1:

import React from "react";
import image from "./image.svg";
import rectangle2 from "./rectangle-2.svg";
import screenshot202510081802302 from "./screenshot-2025-10-08-180230-2.png";
import screenshot202510081803441 from "./screenshot-2025-10-08-180344-1.png";
import textOnAPath from "./text-on-a-path.svg";

export const AndroidCompact = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[340px] min-h-[801px] relative">
      <img
        className="absolute top-0 left-0 w-[340px] h-[801px] aspect-[0.65] object-cover"
        alt="Screenshot"
        src={screenshot202510081802302}
      />

      <img
        className="absolute top-[29px] left-[11px] w-[319px] h-[67px] aspect-[4.75] object-cover"
        alt="Screenshot"
        src={screenshot202510081803441}
      />

      <div className="top-[388px] w-[226px] h-[100px] bg-[#2ae4db] absolute left-[75px]" />

      <div className="absolute top-[416px] left-[133px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        LOGIN
      </div>

      <img
        className="absolute top-[482px] left-[511px] w-[235px] h-[89px]"
        alt="Text on a path"
        src={image}
      />

      <img
        className="absolute top-[503px] left-[511px] w-[226px] h-[91px]"
        alt="Text on a path"
        src={textOnAPath}
      />

      <img
        className="top-[516px] w-[217px] h-[98px] absolute left-[75px]"
        alt="Rectangle"
        src={rectangle2}
      />

      <div className="absolute top-[564px] left-[101px] w-[300px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal] whitespace-nowrap">
        REGISTER
      </div>

      <div className="absolute top-[177px] left-[54px] w-[267px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        SPORTS DAY
      </div>
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

Frame 2

import React from "react";
import screenshot202510081825001 from "./screenshot-2025-10-08-182500-1.png";

export const AndroidCompact = () => {
  return (
    <div className="bg-white w-full min-w-[351px] min-h-[794px] relative">
      <img
        className="absolute top-0 left-0 w-[351px] h-[794px] aspect-[0.52] object-cover"
        alt="Screenshot"
        src={screenshot202510081825001}
      />

      <div className="absolute top-[99px] left-[103px] w-52 [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        EVENTS
      </div>

      <div className="absolute top-[254px] left-[49px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        CRICKET
      </div>

      <div className="absolute top-[386px] left-[49px] w-[285px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        ATHLETICS
      </div>

      <div className="absolute top-[525px] left-[49px] w-[283px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal] whitespace-nowrap">
        BADMITON
      </div>
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

Frame 3
import React from "react";
import rectangle3 from "./rectangle-3.svg";
import screenshot202510081802301 from "./screenshot-2025-10-08-180230-1.png";
import screenshot202510081832171 from "./screenshot-2025-10-08-183217-1.png";

export const AndroidCompact = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[357px] min-h-[794px] relative">
      <img
        className="absolute top-[-54px] left-[-34px] w-[69px] h-[171px] aspect-[0.4] object-cover"
        alt="Screenshot"
        src={screenshot202510081802301}
      />

      <img
        className="absolute top-0 left-0 w-[357px] h-[794px] aspect-[0.6] object-cover"
        alt="Screenshot"
        src={screenshot202510081832171}
      />

      <div className="absolute top-16 left-0 w-[357px] [font-family:'Inter-Regular',Helvetica] font-normal text-[#f81818] text-2xl tracking-[0] leading-[normal]">
        EVENT REGISTRATION DETAILS
      </div>

      <div className="absolute top-[149px] left-[22px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal] whitespace-nowrap">
        TO BE FILLED:
      </div>

      <img
        className="absolute top-[199px] left-[9px] w-[272px] h-[52px]"
        alt="Rectangle"
        src={rectangle3}
      />

      <p className="absolute top-[227px] left-[51px] w-[162px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal]">
        <span className="[font-family:'Inter-Regular',Helvetica] font-normal text-black text-xl tracking-[0]">
          Full name
        </span>

        <span className="text-base">:</span>
      </p>

      <div className="absolute top-[293px] left-[11px] w-[270px] h-[73px] bg-[#edf123]" />

      <div className="absolute top-[338px] left-[51px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal] whitespace-nowrap">
        Gender
      </div>

      <div className="absolute top-[422px] left-[9px] w-[281px] h-[89px] bg-[#f8f40d]" />

      <div className="absolute top-[464px] left-[51px] w-32 [font-family:'Inter-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal]">
        Email-ID
      </div>

      <div className="absolute top-[614px] left-[51px] w-[181px] h-[70px] bg-[#fa1313]" />

      <div className="absolute top-[637px] left-[97px] [font-family:'Inter-Regular',Helvetica] font-normal text-white text-2xl tracking-[0] leading-[normal]">
        REGISTER
      </div>
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
~~~

## OUTPUT:

![alt text](<Screenshot 2025-10-08 190340.png>)
## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
