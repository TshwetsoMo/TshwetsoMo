<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&width=435&lines=Hi+my+name+is+TshwetsoMo" alt="Software Developer" alt="UI/UX Designer" /></a>

<img src="https://github.com/TshwetsoMo/TshwetsoMo/blob/main/TSHWETSO.png?raw=true" alt="Banner Text" width="100%" />

---

### 🧭 About Me
Hi, I am **Tshwetso K. Mokgatlhe**, I'm a multidisciplinary developer and designer based in Pretoria, South Africa. As a final-year Interaction Development and UX Design student at The Open Window Institute, I have learned to combine human-centred design with technical precision to build meaningful digital experiences. I am passionate about innovation, ethics, and accessibility, I explore how technology can empower local communities through creativity and empathy.

---

### 💻 Technical Expertise
- **Frontend Development:** Skilled in building responsive, accessible, and scalable interfaces using **React**, **Next.js**, **TypeScript**, and **TailwindCSS**.  
- **Backend Development:** Proficient in **Node.js**, **Express**, and **ASP.NET Core**, with experience designing RESTful APIs and managing server-side logic.  
- **Database Management:** Strong understanding of **MongoDB**, **PostgreSQL**, and **Firebase Firestore** for efficient data modeling and real-time updates.  
- **Cloud & DevOps:** Familiar with **Azure**, **AWS**, **Docker**, and deployment pipelines for cloud-based full-stack applications.  

---

### 🧰 Tech Stack
<p align="center">
  <!-- Frontend -->
  <img src="https://skillicons.dev/icons?i=react,nextjs,typescript,tailwind,html,css,js" /><br>
  <!-- Backend -->
  <img src="https://skillicons.dev/icons?i=nodejs,express,dotnet,firebase,mongodb,postgresql" /><br>
  <!-- Cloud & Tools -->
  <img src="https://skillicons.dev/icons?i=azure,aws,docker,git,github,figma,xd,illustrator" />
</p>

---

### 🚀 Current Focus
- 🔭 **Working On:** AI integration development.  
- 🌱 **Learning:** Advanced cloud architecture & optimization across **Azure, AWS, and GCP**.   
- ⚡ **Fun Fact:** I want to automate everyday routines with code!

---

### 💎 Featured Projects

#### 🧩 [Bua](https://github.com/TshwetsoMo/bua)
> **Empowering Student Voices Through AI Advocacy**  
> An AI advisor and reporting hub that helps students get answers, surface issues, and drive change at school privately and safely.  
**Tech:** Next.js · TypeScript · Firebase · Gemini AI  
🌍 *Role:* Lead Developer & UX Designer  

---

#### ⏳ [TimeLink](https://github.com/TshwetsoMo/TimeLinked)
> **Time-Capsule Journaling for Future Reflection**  
> Users write, store, and send messages to their future selves and loved ones. Integrating writing to private, public or just friends list.  
**Tech:** React · Firebase · Framer Motion · TailwindCSS · Expo
🎨 *Role:* UX Designer & Full-Stack Developer  

---

#### 💍 [Aureum Elegance](https://github.com/Tsebo200/Aureum-Elegance-Frontend.git)
> **Luxury Jewellery E-Commerce for the Modern Maker**  
> Handmade jewellery platform with real-time inventory, custom order pages, and visual storytelling.  
**Tech:** React · Node.js · Express · MongoDB  
💼 *Role:* Full-Stack Developer  

---

### 🌐 Connect With Me
<p align="left">
  <a href="https://www.linkedin.com/in/tshwetso-mokgatlhe-a032672a0?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app" target="_blank">
    <img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:tshwetsomomokgatlhe98@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/-Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://wa.me/27835758890" target="_blank">
    <img src="https://img.shields.io/badge/-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/>
  </a>
  <a href="https://github.com/TshwetsoMo" target="_blank">
    <img src="https://img.shields.io/badge/-GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://www.behance.net/tshwetsmokgatl1" target="_blank">
    <img src="https://img.shields.io/badge/-Behance-1769FF?style=for-the-badge&logo=behance&logoColor=white"/>
  </a>
</p>

---

### 📈 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=TshwetsoMo&show_icons=true&theme=tokyonight" height="160"/>
  <img src="https://github-readme-streak-stats.herokuapp.com?user=TshwetsoMo&theme=tokyonight" height="160"/>
</p>

### 📊 Top Languages
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=TshwetsoMo&layout=compact&theme=tokyonight" height="160"/>
</p>

---

### 🪄 Quote
> “Do the most.” – *T.K. Mokgatlhe*

I’m always looking to collaborate on **innovative projects** that combine **creativity, social purpose, and technology**.  
Let’s build something that outlasts us. ✨  

---

function setup() {
  createCanvas(710, 400);
  pixelDensity(1);
  describe('Colorful rendering of the Mandelbrot set.');
  background(0);

  // Establish a range of values on the complex plane
  // Different width values change the zoom level
  let w = 4;
  let h = (w * height) / width;

  // Start at negative half the width and height
  let xMin = -w / 2;
  let yMin = -h / 2;

  // Access the pixels[] array
  loadPixels();

  // Set the maximum number of iterations for each point on the complex plane
  let maxIterations = 100;

  // x goes from xMin to xMax
  let xMax = xMin + w;

  // y goes from yMin to yMax
  let yMax = yMin + h;

  // Calculate amount we increment x,y for each pixel
  let dx = (xMax - xMin) / width;
  let dy = (yMax - yMin) / height;

  // Start y
  let y = yMin;
  for (let j = 0; j < height; j += 1) {
    // Start x
    let x = xMin;
    for (let i = 0; i < width; i += 1) {
      // Test whether iteration of z = z^2 + cm diverges
      let a = x;
      let b = y;
      let iterations = 0;
      while (iterations < maxIterations) {
        let aSquared = pow(a, 2);
        let bSquared = pow(b, 2);
        let twoAB = 2.0 * a * b;
        a = aSquared - bSquared + x;
        b = twoAB + y;

        // If the values are too big, stop iteration
        if (dist(aSquared, bSquared, 0, 0) > 16) {
          break;
        }
        iterations += 1;
      }

      // Color each pixel based on how long it takes to get to infinity

      let index = (i + j * width) * 4;

      // Convert number of iterations to range of 0-1
      let normalized = map(iterations, 0, maxIterations, 0, 1);

      // Use square root of normalized value for color interpolation
      let lerpAmount = sqrt(normalized);

      // Set default color to black
      let pixelColor = color(0);

      // Blue
      let startColor = color(47, 68, 159);

      // Light yellow
      let endColor = color(255, 255, 128);

      // If iteration is under the maximum, interpolate a color
      if (iterations < maxIterations) {
        pixelColor = lerpColor(startColor, endColor, lerpAmount);
      }

      // Copy the RGBA values from the color to the pixel
      for (let i = 0; i < 4; i += 1) {
        pixels[index + i] = pixelColor.array()[i] * 255;
      }

      x += dx;
    }
    y += dy;
  }
  updatePixels();
}
