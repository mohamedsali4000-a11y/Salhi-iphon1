<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="متجر iPhone Salhi في برشلونة - هاتفات، كفرات، وإكسسوارات." />
  <title>iPhone Salhi</title>
  <style>
    :root {
      --ink: #18172b;
      --muted: #63657d;
      --line: #e9e7f0;
      --bg: #f7f6fb;
      --white: #ffffff;
      --purple: #7257ed;
      --pink: #ee83b9;
      --green: #1f9b5d;
      --orange: #ffb347;
      --shadow: rgba(24, 23, 43, 0.12);
    }

    * { box-sizing: border-box; }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: var(--bg);
      color: var(--ink);
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button, select {
      font: inherit;
    }

    img {
      max-width: 100%;
      display: block;
    }

    .container {
      width: min(1120px, 92%);
      margin: 0 auto;
    }

    .sr-only {
      position: absolute;
      width: 1px;
      height: 1px;
      padding: 0;
      margin: -1px;
      overflow: hidden;
      clip: rect(0, 0, 0, 0);
      white-space: nowrap;
      border: 0;
    }

    .skip {
      position: absolute;
      inset-inline-start: 12px;
      top: -56px;
      background: white;
      padding: 10px 14px;
      border-radius: 10px;
      z-index: 50;
    }

    .skip:focus {
      top: 12px;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 20;
      background: rgba(255, 255, 255, 0.9);
      border-bottom: 1px solid var(--line);
      backdrop-filter: blur(12px);
    }

    .nav {
      min-height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 18px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
      font-weight: 800;
    }

    .brand-mark {
      width: 42px;
      height: 42px;
      display: grid;
      place-items: center;
      border-radius: 14px;
      background: linear-gradient(135deg, var(--purple), var(--pink));
      color: white;
      font-weight: 800;
    }

    .nav-group {
      display: flex;
      align-items: center;
      gap: 18px;
      flex-wrap: wrap;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 18px;
      color: #4a4f67;
      font-size: 14px;
    }

    .lang-select {
      border: 1px solid var(--line);
      background: white;
      border-radius: 10px;
      padding: 10px 12px;
      min-width: 120px;
    }

    .btn {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      padding: 11px 16px;
      border: 0;
      border-radius: 12px;
      background: var(--purple);
      color: white;
      font-weight: 700;
      cursor: pointer;
      transition: 0.2s ease;
    }

    .btn:hover {
      transform: translateY(-1px);
    }

    .btn.dark {
      background: var(--ink);
    }

    .btn.green {
      background: var(--green);
    }

    .btn.light {
      background: white;
      color: var(--ink);
      border: 1px solid var(--line);
    }

    .hero {
      padding: 72px 0 64px;
      background:
        radial-gradient(circle at 15% 15%, rgba(238, 131, 185, 0.18), transparent 25%),
        radial-gradient(circle at 85% 25%, rgba(114, 87, 237, 0.16), transparent 30%),
        linear-gradient(135deg, #fffef9 0%, #ffffff 100%);
      overflow: hidden;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.15fr 0.85fr;
      gap: 34px;
      align-items: center;
    }

    .tag {
      display: inline-block;
      padding: 8px 14px;
      border-radius: 999px;
      background: #eeeaff;
      color: #563ed4;
      font-size: 13px;
      font-weight: 700;
    }

    h1 {
      margin: 18px 0;
      font-size: clamp(34px, 5vw, 58px);
      line-height: 1.15;
      letter-spacing: -1px;
    }

    .hero-text {
      color: var(--muted);
      line-height: 1.9;
      font-size: 17px;
      max-width: 570px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 25px;
    }

    .hero-image-wrap {
      position: relative;
      display: grid;
      place-items: center;
      min-height: 330px;
    }

    .hero-glow {
      position: absolute;
      width: 310px;
      height: 310px;
      border-radius: 50%;
      background: linear-gradient(135deg, #d9d0ff, #ffdfea);
      filter: blur(3px);
      opacity: 0.9;
    }

    .hero-photo {
      position: relative;
      z-index: 1;
      width: min(100%, 420px);
      height: 340px;
      object-fit: cover;
      border-radius: 28px;
      box-shadow: 0 28px 60px rgba(27, 24, 42, 0.18);
    }

    section {
      padding: 54px 0;
    }

    .heading {
      margin-bottom: 22px;
    }

    .heading h2 {
      margin: 0 0 8px;
      font-size: clamp(26px, 3vw, 36px);
    }

    .heading p {
      margin: 0;
      color: var(--muted);
      line-height: 1.7;
    }

    .note {
      padding: 12px 14px;
      border: 1px solid #f4d7a3;
      background: #fff8e8;
      color: #76540d;
      border-radius: 12px;
      margin-bottom: 22px;
      line-height: 1.7;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 18px;
    }

    .card {
      background: var(--white);
      border: 1px solid var(--line);
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 8px 24px rgba(20, 20, 38, 0.04);
    }

    .card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .card-body {
      padding: 18px;
    }

    .card h3 {
      margin: 0 0 8px;
      font-size: 20px;
    }

    .card p {
      margin: 0 0 15px;
      color: var(--muted);
      line-height: 1.6;
      font-size: 14px;
      min-height: 44px;
    }

    .row {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 10px;
    }

    .price {
      font-size: 20px;
      font-weight: 800;
      white-space: nowrap;
    }

    .info-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 14px;
    }

    .info-box {
      background: var(--white);
      border: 1px solid var(--line);
      border-radius: 16px;
      padding: 20px;
      text-align: center;
    }

    .info-box strong {
      display: block;
      margin-bottom: 6px;
      font-size: 18px;
    }

    .info-box span {
      color: var(--muted);
      font-size: 14px;
    }

    .contact-box {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 18px;
      background: linear-gradient(135deg, #24243d 0%, #6b53e6 100%);
      color: white;
      border-radius: 22px;
      padding: 30px;
    }

    .contact-box h2 {
      margin: 0 0 6px;
      font-size: clamp(24px, 3vw, 32px);
    }

    .contact-box p {
      margin: 0;
      color: #e7e3ff;
      line-height: 1.7;
    }

    .email-line {
      text-align: center;
      color: var(--muted);
      margin-top: 18px;
      line-height: 1.7;
    }

    footer {
      padding: 18px 0 26px;
      text-align: center;
      color: var(--muted);
      font-size: 13px;
    }

    .cart-panel {
      position: fixed;
      inset-inline: auto 18px;
      bottom: 18px;
      width: min(420px, calc(100% - 36px));
      background: white;
      border: 1px solid var(--line);
      border-radius: 18px;
      box-shadow: 0 18px 44px rgba(0, 0, 0, 0.14);
      z-index: 30;
    }

    .cart-panel[hidden] {
      display: none;
    }

    .cart-inner {
      padding: 16px;
    }

    .cart-head {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 10px;
      margin-bottom: 12px;
      font-weight: 800;
    }

    .cart-items {
      list-style: none;
      padding: 0;
      margin: 0;
      max-height: 180px;
      overflow-y: auto;
    }

    .cart-items li {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 10px;
      padding: 8px 0;
      border-bottom: 1px solid var(--line);
    }

    .cart-items li:last-child {
      border-bottom: 0;
    }

    .cart-total {
      margin-top: 12px;
      padding-top: 12px;
      border-top: 1px solid var(--line);
      font-weight: 800;
    }

    .cart-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 14px;
    }

    @media (max-width: 760px) {
      .nav {
        min-height: 64px;
      }

      .nav-links {
        display: none;
      }

      .nav-group {
        gap: 10px;
      }

      .hero {
        padding-top: 48px;
      }

      .hero-grid {
        grid-template-columns: 1fr;
        text-align: center;
      }

      .hero-text {
        margin-inline: auto;
      }

      .actions {
        justify-content: center;
      }

      .products {
        grid-template-columns: 1fr;
      }

      .info-grid {
        grid-template-columns: 1fr;
      }

      .contact-box {
        flex-direction: column;
        align-items: flex-start;
        text-align: start;
      }
    }

    @media (min-width: 761px) and (max-width: 980px) {
      .products {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }
  </style>
</head>
<body>
  <a class="skip" href="#main-content">تجاوز إلى المحتوى</a>

  <header>
    <div class="container nav">
      <a class="brand" href="#" aria-label="الصفحة الرئيسية">
        <span class="brand-mark">S</span>
        <span>iPhone Salhi</span>
      </a>

      <div class="nav-group">
        <nav class="nav-links" aria-label="القائمة الرئيسية">
          <a href="#phones" data-i18n="navPhones">الهواتف</a>
          <a href="#cases" data-i18n="navCases">الكفرات</a>
          <a href="#delivery" data-i18n="navDelivery">التوصيل</a>
          <a href="#contact" data-i18n="navContact">تواصل معنا</a>
        </nav>

        <label class="sr-only" for="languageSelect">Language</label>
        <select id="languageSelect" class="lang-select" aria-label="اختيار اللغة">
          <option value="ar">العربية</option>
          <option value="es">Español</option>
          <option value="en">English</option>
        </select>

        <button class="btn dark" id="cartToggle" aria-expanded="false" aria-controls="cartPanel">
          <span data-i18n="cart">السلة</span>
          (<span id="cartCount">0</span>)
        </button>
      </div>
    </div>
  </header>

  <main id="main-content">
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="tag">Barcelona • iPhone</span>
          <h1 data-i18n="heroTitle">هواتف وإكسسوارات بستايل كيعجبك</h1>
          <p class="hero-text" data-i18n="heroText">
            اختار iPhone ديالك والكفر المناسب. هاد الصفحة تجريبية فقط، ما كاينش طلب حقيقي ولا دفع فعلي.
          </p>

          <div class="actions">
            <a class="btn" href="#phones" data-i18n="btnShop">تسوق الآن</a>
            <a class="btn light" href="#cases" data-i18n="btnCases">شوف الكفرات</a>
          </div>
        </div>

        <div class="hero-image-wrap">
          <div class="hero-glow" aria-hidden="true"></div>
          <img
            class="hero-photo"
            src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?auto=format&fit=crop&w=1200&q=85"
            alt="هاتف ذكي على خلفية زاهية"
          />
        </div>
      </div>
    </section>

    <section id="phones">
      <div class="container">
        <div class="heading">
          <h2 data-i18n="phonesTitle">هواتف iPhone</h2>
          <p data-i18n="phonesSubtitle">الأثمنة تجريبية، وتأكد من التوفر قبل الشراء.</p>
        </div>

        <div class="note" role="note" data-i18n="demoNote">
          متجر تجريبي: لا توجد عملية بيع أو دفع حقيقية. الصور توضيحية، وقد لا تطابق الموديل بشكل دقيق.
        </div>

        <div class="products">
          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1592750475338-74b7b21085ab?auto=format&fit=crop&w=900&q=85"
              alt="iPhone 18 Pro"
            />
            <div class="card-body">
              <h3>iPhone 18 Pro</h3>
              <p data-i18n="iphone18Desc">موديل فاخر، ألوان متعددة، سعر تجريبي حسب التوفر.</p>
              <div class="row">
                <span class="price">1,111€</span>
                <button class="btn add" data-name="iPhone 18 Pro" data-price="1111">
                  <span data-i18n="addToCart">زيد للسلة</span>
                </button>
              </div>
            </div>
          </article>

          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?auto=format&fit=crop&w=900&q=85"
              alt="iPhone 16"
            />
            <div class="card-body">
              <h3>iPhone 16</h3>
              <p data-i18n="iphone16Desc">تحديث حديث ومناسب لمن يريد هاتف سريع ومريح في الاستخدام.</p>
              <div class="row">
                <span class="price">719€</span>
                <button class="btn add" data-name="iPhone 16" data-price="719">
                  <span data-i18n="addToCart">زيد للسلة</span>
                </button>
              </div>
            </div>
          </article>

          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1598327105666-5b89351aff97?auto=format&fit=crop&w=900&q=85"
              alt="iPhone 15"
            />
            <div class="card-body">
              <h3>iPhone 15</h3>
              <p data-i18n="iphone15Desc">حل عملي وذكي، مناسب للمستخدمين اللي يحتاجون تجربة ممتازة.</p>
              <div class="row">
                <span class="price">449€</span>
                <button class="btn add" data-name="iPhone 15" data-price="449">
                  <span data-i18n="addToCart">زيد للسلة</span>
                </button>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="cases">
      <div class="container">
        <div class="heading">
          <h2 data-i18n="casesTitle">كفرات iPhone</h2>
          <p data-i18n="casesSubtitle">ألوان متعددة، مرونة في التصميم، وحماية يومية.</p>
        </div>

        <div class="products">
          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1603313011105-320f26a4f6f6?auto=format&fit=crop&w=900&q=85"
              alt="كفر هاتف ألوان"
            />
            <div class="card-body">
              <h3 data-i18n="case1">كفر ملون</h3>
              <p data-i18n="case1Desc">ألوان جذابة تناسب كل طابع.</p>
              <div class="row">
                <span class="price">5€</span>
                <button class="btn add" data-name="كفر ملون" data-price="5">
                  <span data-i18n="addToCart">زيد للسلة</span>
                </button>
              </div>
            </div>
          </article>

          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1605236453806-6ff36851218e?auto=format&fit=crop&w=900&q=85"
              alt="كفر حماية"
            />
            <div class="card-body">
              <h3 data-i18n="case2">كفر حماية</h3>
              <p data-i18n="case2Desc">حماية أقوى مع تصميم أنيق.</p>
              <div class="row">
                <span class="price">10€</span>
                <button class="btn add" data-name="كفر حماية" data-price="10">
                  <span data-i18n="addToCart">زيد للسلة</span>
                </button>
              </div>
            </div>
          </article>

          <article class="card">
            <img
              src="https://images.unsplash.com/photo-1601593346740-925612772716?auto=format&fit=crop&w=900&q=85"
              alt="كفر فاخر"
            />
            <div class="card-body">
              <h3 data-i18n="case3">كفر فاخر</h3>
              <p data-i18n="case3Desc">تصميم خاص ومميز للهواتف الحديثة.</p>
              <div class="row">
                <span class="price">15€</span>
                <button class="btn add" data-name="كفر فاخر" data-price="15">
                  <span data-i18n="addToCart">زيد للسلة</span>
                </button>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="delivery">
      <div class="container">
        <div class="info-grid">
          <div class="info-box">
            <strong data-i18n="info1Title">📍 برشلونة</strong>
            <span data-i18n="info1Text">خدمة توصيل داخل برشلونة</span>
          </div>

          <div class="info-box">
            <strong data-i18n="info2Title">🚚 7€</strong>
            <span data-i18n="info2Text">سعر التوصيل داخل المدينة</span>
          </div>

          <div class="info-box">
            <strong data-i18n="info3Title">🎨 ألوان متنوعة</strong>
            <span data-i18n="info3Text">اختيار من الألوان المتوفرة</span>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="contact-box">
          <div>
            <h2 data-i18n="contactTitle">بغيتي تشتري أو تستفسر؟</h2>
            <p data-i18n="contactText">تواصل معنا عبر واتساب أو البريد الإلكتروني.</p>
          </div>

          <a
            class="btn green"
            href="https://wa.me/34666784846?text=Salam%2C%20bghit%20n3ref%20details%20dyal%20produits"
            data-i18n="contactBtn"
          >
            واتساب
          </a>
        </div>

        <p class="email-line">
          <span data-i18n="emailLabel">البريد الإلكتروني:</span>
          <a href="mailto:mohammedsalhi4000@gmail.com">mohammedsalhi4000@gmail.com</a>
        </p>
      </div>
    </section>
  </main>

  <aside class="cart-panel" id="cartPanel" hidden aria-live="polite" aria-label="السلة">
    <div class="cart-inner">
      <div class="cart-head">
        <span data-i18n="cartTitle">السلة التجريبية</span>
        <button class="btn light" id="closeCart" data-i18n="closeCart">إغلاق</button>
      </div>

      <ul id="cartItems" class="cart-items"></ul>

      <div class="cart-total">
        <span data-i18n="totalLabel">المجموع:</span>
        <span id="cartTotal">0</span>€
      </div>

      <div class="cart-actions">
        <button class="btn" id="checkoutBtn" data-i18n="checkoutBtn">متابعة تجريبية</button>
        <button class="btn light" id="clearCartBtn" data-i18n="clearCartBtn">إفراغ السلة</button>
      </div>
    </div>
  </aside>

  <footer>
    © 2026 iPhone Salhi — Barcelona
  </footer>

  <script>
    const translations = {
      ar: {
        navPhones: "الهواتف",
        navCases: "الكفرات",
        navDelivery: "التوصيل",
        navContact: "تواصل معنا",
        cart: "السلة",
        heroTitle: "هواتف وإكسسوارات بستايل كيعجبك",
        heroText: "اختار iPhone ديالك والكفر المناسب. هاد الصفحة تجريبية فقط، ما كاينش طلب حقيقي ولا دفع فعلي.",
        btnShop: "تسوق الآن",
        btnCases: "شوف الكفرات",
        phonesTitle: "هواتف iPhone",
        phonesSubtitle: "الأثمنة تجريبية، وتأكد من التوفر قبل الشراء.",
        demoNote: "متجر تجريبي: لا توجد عملية بيع أو دفع حقيقية. الصور توضيحية، وقد لا تطابق الموديل بشكل دقيق.",
        iphone18Desc: "موديل فاخر، ألوان متعددة، سعر تجريبي حسب التوفر.",
        iphone16Desc: "تحديث حديث ومناسب لمن يريد هاتف سريع ومريح في الاستخدام.",
        iphone15Desc: "حل عملي وذكي، مناسب للمستخدمين اللي يحتاجون تجربة ممتازة.",
        addToCart: "زيد للسلة",
        casesTitle: "كفرات iPhone",
        casesSubtitle: "ألوان متعددة، مرونة في التصميم، وحماية يومية.",
        case1: "كفر ملون",
        case1Desc: "ألوان جذابة تناسب كل طابع.",
        case2: "كفر حماية",
        case2Desc: "حماية أقوى مع تصميم أنيق.",
        case3: "كفر فاخر",
        case3Desc: "تصميم خاص ومميز للهواتف الحديثة.",
        info1Title: "📍 برشلونة",
        info1Text: "خدمة توصيل داخل برشلونة",
        info2Title: "🚚 7€",
        info2Text: "سعر التوصيل داخل المدينة",
        info3Title: "🎨 ألوان متنوعة",
        info3Text: "اختيار من الألوان المتوفرة",
        contactTitle: "بغيتي تشتري أو تستفسر؟",
        contactText: "تواصل معنا عبر واتساب أو البريد الإلكتروني.",
        contactBtn: "واتساب",
        emailLabel: "البريد الإلكتروني:",
        cartTitle: "السلة التجريبية",
        closeCart: "إغلاق",
        totalLabel: "المجموع:",
        checkoutBtn: "متابعة تجريبية",
        clearCartBtn: "إفراغ السلة"
      },
      es: {
        navPhones: "Teléfonos",
        navCases: "Fundas",
        navDelivery: "Envío",
        navContact: "Contacto",
        cart: "Carrito",
        heroTitle: "iPhones y accesorios con estilo",
        heroText: "Elige tu iPhone y la funda ideal. Esta página es solo una demostración, sin pedidos ni pagos reales.",
        btnShop: "Comprar ahora",
        btnCases: "Ver fundas",
        phonesTitle: "Teléfonos iPhone",
        phonesSubtitle: "Los precios son de demostración y deben confirmarse antes de comprar.",
        demoNote: "Tienda de demostración: no se realizan compras ni pagos reales. Las imágenes son ilustrativas.",
        iphone18Desc: "Modelo premium con varios colores y precio de demostración según disponibilidad.",
        iphone16Desc: "Actualización moderna, ideal para quienes buscan velocidad y comodidad.",
        iphone15Desc: "Solución práctica y elegante para un uso diario muy cómodo.",
        addToCart: "Añadir al carrito",
        casesTitle: "Fundas para iPhone",
        casesSubtitle: "Múltiples colores, diseño flexible y protección diaria.",
        case1: "Funda colorida",
        case1Desc: "Colores atractivos para cualquier estilo.",
        case2: "Funda de protección",
        case2Desc: "Protección reforzada con diseño elegante.",
        case3: "Funda premium",
        case3Desc: "Diseño especial para teléfonos modernos.",
        info1Title: "📍 Barcelona",
        info1Text: "Servicio de entrega en Barcelona",
        info2Title: "🚚 7€",
        info2Text: "Precio del envío dentro de la ciudad",
        info3Title: "🎨 Colores variados",
        info3Text: "Variedad de colores disponibles",
        contactTitle: "¿Quieres comprar o consultar?",
        contactText: "Contáctanos por WhatsApp o correo electrónico.",
        contactBtn: "WhatsApp",
        emailLabel: "Correo electrónico:",
        cartTitle: "Carrito de prueba",
        closeCart: "Cerrar",
        totalLabel: "Total:",
        checkoutBtn: "Continuar de prueba",
        clearCartBtn: "Vaciar carrito",
      },
      en: {
        navPhones: "Phones",
        navCases: "Cases",
        navDelivery: "Delivery",
        navContact: "Contact",
        cart: "Cart",
        heroTitle: "iPhones and accessories in style",
        heroText: "Choose your iPhone and the perfect case. This page is only a demo and has no real purchases or payments.",
        btnShop: "Shop now",
        btnCases: "View cases",
        phonesTitle: "iPhone Phones",
        phonesSubtitle: "Prices are demo only and should be confirmed before purchase.",
        demoNote: "Demo store: there are no real sales or payments. Images are illustrative only.",
        iphone18Desc: "Premium model with several colors and demo pricing based on stock.",
        iphone16Desc: "Modern update, ideal for users who want speed and comfort.",
        iphone15Desc: "A practical and stylish option for everyday use.",
        addToCart: "Add to cart",
        casesTitle: "iPhone Cases",
        casesSubtitle: "Multiple colors, flexible design, and daily protection.",
        case1: "Colorful case",
        case1Desc: "Attractive colors for every style.",
        case2: "Protective case",
        case2Desc: "Stronger protection with a sleek design.",
        case3: "Premium case",
        case3Desc: "Special design for modern smartphones.",
        info1Title: "📍 Barcelona",
        info1Text: "Delivery service in Barcelona",
        info2Title: "🚚 €7",
        info2Text: "City delivery rate",
        info3Title: "🎨 Various colors",
        info3Text: "Choice of available colors",
        contactTitle: "Want to buy or ask a question?",
        contactText: "Contact us via WhatsApp or email.",
        contactBtn: "WhatsApp",
        emailLabel: "Email:",
        cartTitle: "Demo Cart",
        closeCart: "Close",
        totalLabel: "Total:",
        checkoutBtn: "Continue demo",
        clearCartBtn: "Empty cart",
      }
    };

    const languageSelect = document.getElementById("languageSelect");
    const cart = [];
    const cartPanel = document.getElementById("cartPanel");
    const cartCount = document.getElementById("cartCount");
    const cartItems = document.getElementById("cartItems");
    const cartTotal = document.getElementById("cartTotal");
    const cartToggle = document.getElementById("cartToggle");
    const closeCart = document.getElementById("closeCart");
    const clearCartBtn = document.getElementById("clearCartBtn");
    const checkoutBtn = document.getElementById("checkoutBtn");

    function updateCartUI() {
      cartItems.innerHTML = "";
      let total = 0;

      cart.forEach((item, index) => {
        total += Number(item.price);

        const li = document.createElement("li");
        const label = document.createElement("span");
        const removeBtn = document.createElement("button");
        removeBtn.type = "button";
        removeBtn.className = "btn light";
        removeBtn.textContent = "✕";
        removeBtn.setAttribute("aria-label", `Remove ${item.name}`);
        removeBtn.addEventListener("click", () => {
          cart.splice(index, 1);
          updateCartUI();
        });

        label.textContent = `${item.name} — ${item.price}€`;
        li.appendChild(label);
        li.appendChild(removeBtn);
        cartItems.appendChild(li);
      });

      cartCount.textContent = cart.length;
      cartTotal.textContent = total;
    }

    document.querySelectorAll(".add").forEach((button) => {
      button.addEventListener("click", () => {
        const name = button.dataset.name;
        const price = Number(button.dataset.price);

        cart.push({ name, price });
        updateCartUI();
        cartPanel.hidden = false;
        cartToggle.setAttribute("aria-expanded", "true");
      });
    });

    cartToggle.addEventListener("click", () => {
      const isHidden = cartPanel.hidden;
      cartPanel.hidden = !isHidden;
      cartToggle.setAttribute("aria-expanded", String(!isHidden));
    });

    closeCart.addEventListener("click", () => {
      cartPanel.hidden = true;
      cartToggle.setAttribute("aria-expanded", "false");
    });

    clearCartBtn.addEventListener("click", () => {
      cart.length = 0;
      updateCartUI();
    });

    checkoutBtn.addEventListener("click", () => {
      alert("هذا متجر تجريبي فقط — لا توجد عملية طلب حقيقية ولا دفع فعلي.");
    });

    function setLanguage(lang) {
      const selected = translations[lang] ? lang : "ar";
      document.documentElement.lang = selected;
      document.documentElement.dir = selected === "ar" ? "rtl" : "ltr";

      document.querySelectorAll("[data-i18n]").forEach((el) => {
        const key = el.dataset.i18n;
        if (translations[selected][key]) {
          el.textContent = translations[selected][key];
        }
      });

      languageSelect.value = selected;
      localStorage.setItem("storeLanguage", selected);
    }

    languageSelect.addEventListener("change", (event) => {
      setLanguage(event.target.value);
    });

    const savedLanguage = localStorage.getItem("storeLanguage") || "ar";
    setLanguage(savedLanguage);
    updateCartUI();
  </script>
</body>
</html>
