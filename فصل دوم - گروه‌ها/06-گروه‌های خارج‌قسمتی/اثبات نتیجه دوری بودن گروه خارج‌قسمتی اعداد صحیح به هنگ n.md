---
uid: "MK-02SG98"
kind: "proof"
subtype: "rigorous"
slug: "proof-integers-modulo-n-quotient-group-is-cyclic"
status: "canonical"
schema_version: "1.1.0"
title_fa: "اثبات نتیجه دوری بودن گروه خارج‌قسمتی اعداد صحیح به هنگ n"
title_en: "Proof of Corollary on Cyclic Nature of Integers Modulo n Quotient Group"
aliases:
  - "برهان دوری بودن Z بر nZ"
  - "اثبات نتیجه ۳۳.۲"
  - "Proof Integers Modulo N Quotient Group Is Cyclic"
slogan_fa: 'اثبات صوری از طریق دوری بودن $\mathbb{Z} = \langle 1 \rangle$، انتقال مولد توسط قضیه ۳۲.۲(پ) و تعیین دقیق مرتبه $n$ با قضیه تقسیم.'
slogan_en: 'Formal proof via cyclicity of $\mathbb{Z} = \langle 1 \rangle$, generator transfer by Theorem 32.2(c), and exact order determination $n$ via the division algorithm.'
msc_primary: "20-01"
tracks:
  - "pure_university"
theory_scope: "[[algebraic-structures-foundations]]"
level: "L3_undergrad_core"
bloom_cognitive: "evaluate"
bloom_knowledge: "procedural"
dok: 4
proof_methods:
  - "direct"
  - "algebraic"
is_constructive: true
authors:
  - "علیرضا علائیان"
  - "process:ai-agent/1.0"
created: "2026-11-23T03:00:00Z"
updated: "2026-11-23T03:00:00Z"
tags:
  - "جبر_مجرد"
  - "نظریه_گروه‌ها"
  - "فصل_دوم"
  - "اثبات"
  - "برهان_صوری"
  - "گروه_دوری"
  - "اعداد_صحیح"
rel_proves:
  - "[[نتیجه دوری بودن گروه خارج‌قسمتی اعداد صحیح به هنگ n]]"
rel_depends_proof:
  - "[[قضیه خواص ساختاری گروه خارج‌قسمتی]]"
  - "[[تعریف گروه دوری و مولد]]"
---

# 🔬 اثبات نتیجه دوری بودن گروه خارج‌قسمتی اعداد صحیح به هنگ n

> [!abstract] نقشه و ایده کلیدی برهان (Proof Strategy & Core Trick)
> * **راهبرد کلی:** برهان بر پایه دو مرحله روشن و منظم استوار است:
>   1. **اثبات دوری بودن و تعیین مولد:** استفاده مستقیم از بند (پ) قضیه ۳۲.۲ که انتقال مولد از گروه مادر به گروه خارج‌قسمتی را تضمین می‌کند.
>   2. **محاسبه دقیق مرتبه و متمایز بودن اعضا:** نشان دادن این‌که کوچک‌ترین ضریب مثبت که مولد را به همانی (رده صفر) تبدیل می‌کند، دقیقاً خود عدد $n$ است (ص ۲۹ جزوه علائیان).

---

## ۱. برهان گام‌به‌گام و صوری (Rigorous Proof Steps)

> [!PROOF] متن کامل برهان نتیجه ۳۳.۲ جزوه علائیان
> فرض کنید $(\mathbb{Z}, +)$ [[تعریف گروه|گروه جمعی اعداد صحیح]] و $n \in \mathbb{N}$ عددی طبیعی ($n \geqslant 1$) باشد.  
> زیرگروه $n\mathbb{Z} = \{ nk \mid k \in \mathbb{Z} \}$ را در نظر می‌گیریم.
>
> ---
>
> ### گام اول: نرمال بودن زیرگروه $n\mathbb{Z}$
> چون گروه $(\mathbb{Z}, +)$ جابجایی (آبلی) است، بنا به ویژگی‌های پایه‌ای، هر زیرگروهی از یک گروه آبلی، نرمال است:
> 
> $$n\mathbb{Z} \trianglelefteq \mathbb{Z}$$
> 
> بنابراین گروه خارج‌قسمتی $\mathbb{Z}/n\mathbb{Z}$ تحت عمل جمع رده‌ها طبق قضیه ۳۱.۲ کاملاً خوش‌تعریف است.
>
> ---
>
> ### گام دوم: انتقال ویژگی دوری بودن
> می‌دانیم که گروه جمعی اعداد صحیح $\mathbb{Z}$ یک گروه دوری است که توسط عدد ۱ تولید می‌شود:
> 
> $$\mathbb{Z} = \langle 1 \rangle = \{ m \cdot 1 \mid m \in \mathbb{Z} \}$$
> 
> اکنون بند (پ) از [[قضیه خواص ساختاری گروه خارج‌قسمتی|قضیه ۳۲.۲ جزوه]] را فراخوانی می‌کنیم:
> «اگر $G$ دوری با مولد $g$ باشد ($G = \langle g \rangle$) و $N \trianglelefteq G$، آنگاه $G/N$ نیز دوری بوده و توسط $gN$ تولید می‌شود ($G/N = \langle gN \rangle$).»
> 
> با جایگذاری $G = \mathbb{Z}$، $g = 1$ و $N = n\mathbb{Z}$ در این حکم، بلافاصله نتیجه می‌شود:
> 
> $$\mathbb{Z}/n\mathbb{Z} = \langle 1 + n\mathbb{Z} \rangle$$
> 
> یعنی گروه خارج‌قسمتی $\mathbb{Z}/n\mathbb{Z}$ دوری است و توسط هم‌مجموعه جمعی $1 + n\mathbb{Z}$ تولید می‌شود.
>
> ---
>
> ### گام سوم: تعیین مرتبه مولد و تعداد عناصر
> طبق تعریف مرتبه عنصر در نماد جمعی، مرتبه رده $1 + n\mathbb{Z}$ برابر با کوچک‌ترین عدد صحیح مثبت $k \in \mathbb{N}$ است به طوری که حاصلضرب اسکالر آن با مولد، برابر با عضو خنثی گروه یعنی $0 + n\mathbb{Z} = n\mathbb{Z}$ گردد:
> 
> $$k \cdot (1 + n\mathbb{Z}) = 0 + n\mathbb{Z} \iff (k \cdot 1) + n\mathbb{Z} = n\mathbb{Z} \iff k \in n\mathbb{Z}$$
> 
> تعلق $k \in n\mathbb{Z}$ به این معناست که $k$ مضربی از $n$ است:
> 
> $$n \mid k$$
> 
> از میان تمام اعداد صحیح مثبت، کوچک‌ترین عددی که مضرب $n$ باشد، خود عدد $n$ است.  
> بنابراین مرتبه مولد $1 + n\mathbb{Z}$ دقیقاً برابر با $n$ است:
> 
> $$|1 + n\mathbb{Z}| = n$$
> 
> چون مرتبه یک گروه دوری متناهی همواره با مرتبه مولد آن برابر است:
> 
> $$|\mathbb{Z}/n\mathbb{Z}| = |\langle 1 + n\mathbb{Z} \rangle| = n$$
>
> ---
>
> ### گام چهارم: فهرست عناصر متمایز با قضیه تقسیم
> برای هر $z \in \mathbb{Z}$، با تقسیم $z$ بر $n$ داریم $z = nq + r$ با $0 \leqslant r < n$. پس:
> 
> $$z + n\mathbb{Z} = (nq + r) + n\mathbb{Z} = r + (nq + n\mathbb{Z}) = r + n\mathbb{Z}$$
> 
> چون $0 \leqslant r \leqslant n - 1$، عناصر متمایز گروه عبارتند از:
> 
> $$\mathbb{Z}/n\mathbb{Z} = \{ n\mathbb{Z} , 1 + n\mathbb{Z} , 2 + n\mathbb{Z} , \dots , (n-1) + n\mathbb{Z} \}$$
> 
> و اثبات به پایان می‌رسد.
> 
> $$\blacksquare$$

---

## ۲. تحلیل محل مصرف فرض‌ها و گلوگاه‌ها (Hypotheses Usage & Bottlenecks)

* **تولیدپذیری $\mathbb{Z}$ توسط عدد ۱:**  
  برهان مستقیماً متکی بر این واقعیت است که ۱ تک‌مولد $\mathbb{Z}$ با توان‌های جمعی است. اگر از زیرگروهی دیگر مانند $2\mathbb{Z}$ آغاز می‌کردیم، خارج‌قسمت آن بر $2n\mathbb{Z}$ همچنان دوری بود اما توسط ۲ تولید می‌شد.
* **الگوریتم اقلیدسی:**  
  یکتایی باقیمانده‌ها در بازه $[0, n-1]$ گلوگاه اثبات عدم هم‌پوشانی و متمایز بودن عناصر $n$گانه خارج‌قسمت است.

---

## ۳. دام‌ها و نکات باریک برهان (Subtleties & Pitfalls)

* **تفاوت ساختاری با مرتبه بی‌نهایت:**  
  اگر $n=0$ باشد، $0\mathbb{Z} = \{0\}$ و کوچک‌ترین عدد مثبت مضرب صفر وجود ندارد؛ در نتیجه مرتبه مولد $1 + \{0\}$ بی‌نهایت است و خارج‌قسمت با خود $\mathbb{Z}$ یک‌ریخت می‌گردد.
