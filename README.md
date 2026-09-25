# 🌿 MindEase AI — 24/7 Student Mental Health Companion

MindEase AI is a 24/7 GenAI-powered mental health companion designed specifically for student well-being[cite: 1]. It provides immediate, judgment-free, and accessible support to help students navigate academic burnout, placement anxiety, and campus stress[cite: 1].

![MindEase AI Banner](https://via.placeholder.com/1200x400/050f0c/10b981?text=MindEase+AI+-+Accessible+Health+%26+Wellness)

---

## ⚡ Key Features

* **24/7 GenAI Support:** Instant, empathetic conversational AI tailored for late-night exam stress and academic pressure.
* **Student-Centric Context:** Speaks student-friendly language with contextual memory around exams, placements, and hostel life.
* **Safety & Crisis Protocols:** Built-in guardrails and real-time helpline escalation for severe distress.
* **Micro-Interventions:** Integrated CBT grounding exercises, guided breathing, and mood tracking.
* **100% Free & Anonymous:** Lowers friction and stigma by eliminating appointment barriers and high therapy costs.

---
## 🛠️ Tech Stack

### **Frontend**
* **Framework:** [Next.js](https://nextjs.org/) (App Router, TypeScript)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **UI Components:** [shadcn/ui](https://ui.shadcn.com/)
* **Animations:** [Framer Motion](https://www.framer.com/motion/) / [GSAP](https://greensock.com/gsap/) with ScrollTrigger
* **Icons:** [Lucide React](https://lucide.dev/)

### **Backend & Database**
* **BaaS:** [Supabase](https://supabase.com/) / [Appwrite](https://appwrite.io/)
  * Auth (Anonymous & Email Login)
  * Database (PostgreSQL / Appwrite DB)
  * Realtime Subscriptions

---

## 📁 Project Structure

```text
mindease-ai/
├── public/                  # Static assets & icons
├── src/
│   ├── app/                 # Next.js App Router routes
│   │   ├── (auth)/          # Authentication routes
│   │   ├── chat/            # Main AI Chat interface
│   │   ├── dashboard/       # Mood tracking & self-help tools
│   │   ├── api/             # Next.js API endpoints / AI streams
│   │   ├── layout.tsx       # Root layout
│   │   └── page.tsx         # Landing page
│   ├── components/
│   │   ├── ui/              # shadcn/ui components
│   │   ├── landing/         # Hero, Stats, Scenarios, FAQ sections
│   │   ├── chat/            # Chat messages, input, and controls
│   │   └── animations/      # Framer Motion / GSAP wrappers
│   ├── lib/
│   │   ├── supabase/        # Supabase client & helper functions
│   │   ├── appwrite/        # Appwrite client & helper functions
│   │   └── utils.ts         # Utility functions (cn helper)
│   ├── styles/
│   │   └── globals.css      # Tailwind & global CSS variables
│   └── types/               # TypeScript interfaces & definitions
├── .env.example
