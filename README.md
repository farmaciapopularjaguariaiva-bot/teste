# teste
teste exlusão

<!doctype html>
<html lang="pt-BR" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Catálogo de Fraldas - Farmácia Popular</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&amp;family=Nunito:wght@300;400;600;700&amp;display=swap" rel="stylesheet">
  <style>
    body {
      box-sizing: border-box;
    }

    .font-fredoka {
      font-family: 'Fredoka', sans-serif;
    }

    .font-nunito {
      font-family: 'Nunito', sans-serif;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
    }

    @keyframes slide-in {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes pulse-soft {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.7; }
    }

    @keyframes shimmer {
      0% { transform: translateX(-100%); }
      100% { transform: translateX(100%); }
    }

    .animate-float {
      animation: float 3s ease-in-out infinite;
    }

    .animate-slide-in {
      animation: slide-in 0.8s ease-out;
    }

    .animate-pulse-soft {
      animation: pulse-soft 2s ease-in-out infinite;
    }

    .brand-card {
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .brand-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 28px rgba(0, 0, 0, 0.12);
    }

    .brand-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: linear-gradient(135deg, rgba(255,255,255,0.3), rgba(255,255,255,0));
      opacity: 0;
      transition: opacity 0.3s ease;
    }

    .brand-card:hover::before {
      opacity: 1;
    }

    .size-button {
      transition: all 0.2s ease;
      cursor: pointer;
      border-radius: 12px;
      padding: 12px 20px;
      font-weight: 600;
      font-size: 14px;
      border: 2px solid transparent;
      background-color: #F5F5F5;
      color: #666;
      position: relative;
      overflow: hidden;
    }

    .size-button:hover {
      background-color: #EFEFEF;
      transform: scale(1.05);
    }

    .size-button.active {
      color: #FFFFFF;
      border-color: currentColor;
    }

    .size-button.active::after {
      content: '✓';
      position: absolute;
      right: 8px;
      top: 50%;
      transform: translateY(-50%);
      font-weight: bold;
    }

    .shine-effect {
      position: relative;
      overflow: hidden;
    }

    .shine-effect::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
      animation: shimmer 2s infinite;
    }

    .feature-icon {
      font-size: 28px;
      margin-bottom: 12px;
    }

    .gradient-bg-soft {
      background: linear-gradient(135deg, #FFEEF5 0%, #E8F4F8 50%, #F0F5FF 100%);
    }

    .modal-hidden {
      display: none;
    }

    .modal-visible {
      display: flex;
    }

    .photo-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 12px;
    }

    .photo-item {
      cursor: pointer;
      border-radius: 12px;
      overflow: hidden;
      transition: all 0.3s ease;
      border: 2px solid transparent;
    }

    .photo-item:hover {
      transform: scale(1.05);
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }

    .photo-item img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      display: block;
    }
  </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="h-full font-nunito bg-white">
  <div id="catalog-container" class="h-full w-full overflow-auto">
   <div class="min-h-full w-full gradient-bg-soft"><!-- Header Section -->
    <div class="relative overflow-hidden pt-8 px-4 pb-12 shine-effect" style="background: linear-gradient(135deg, #87CEEB 0%, #A8D8EA 50%, #AAE4E9 100%);"><!-- Floating Decorative Elements -->
     <div class="absolute top-6 left-8 text-4xl animate-float">
      👶
     </div>
     <div class="absolute top-8 right-10 text-3xl animate-float" style="animation-delay: 0.5s;">
      🍼
     </div>
     <div class="absolute bottom-4 left-1/3 text-3xl animate-float" style="animation-delay: 1s;">
      ����
     </div>
     <div class="absolute bottom-6 right-1/4 text-2xl animate-float" style="animation-delay: 1.5s;">
      ��
     </div>
     <div class="absolute top-20 right-1/3 text-2xl animate-float" style="animation-delay: 0.8s;">
      🎀
     </div><!-- Main Content -->
     <div class="relative z-10 max-w-6xl mx-auto text-center"><!-- Pharmacy Badge -->
      <div class="inline-block mb-4 px-4 py-2 rounded-full" style="background-color: rgba(255,255,255,0.9);">
       <p class="text-sm font-semibold tracking-wide" style="color: #87CEEB; text-transform: uppercase; letter-spacing: 0.1em;">🏥 Farmácia Popular</p>
      </div><!-- Main Title -->
      <h1 id="catalog-title" class="font-fredoka text-5xl md:text-6xl font-bold mt-4 animate-slide-in" style="color: #FFFFFF; text-shadow: 0 2px 10px rgba(0,0,0,0.1);">Catálogo de Fraldas</h1><!-- Subtitle -->
      <p id="subtitle-text" class="text-lg md:text-xl mt-4 animate-slide-in font-nunito" style="color: rgba(255,255,255,0.95); animation-delay: 0.1s;">Escolha o tamanho ideal para seu bebê</p><!-- Decorative Line -->
      <div class="w-32 h-1 mx-auto mt-6 animate-slide-in" style="background-color: rgba(255,255,255,0.7); animation-delay: 0.2s;"></div>
     </div>
    </div><!-- Main Content -->
    <div class="px-4 py-12 max-w-7xl mx-auto"><!-- Introduction Section -->
     <div class="text-center mb-12 animate-slide-in" style="animation-delay: 0.3s;">
      <p class="text-lg font-nunito" style="color: #555; max-width: 600px; margin: 0 auto;">Oferecemos as melhores marcas de fraldas do mercado com qualidade premium e conforto garantido para seu bebê.</p>
     </div><!-- Brands Section -->
     <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 mb-16"><!-- Mili Love Care Brand -->
      <div class="brand-card animate-slide-in rounded-2xl p-8 shadow-lg" style="background: linear-gradient(135deg, #FFF5F9 0%, #FFE8F1 100%); border: 2px solid #FFB6D9; animation-delay: 0.1s; position: relative;"><!-- GIGA Badge -->
       <div style="position: absolute; top: -12px; right: 20px; background: linear-gradient(135deg, #FFB6D9, #FF99BB); color: white; padding: 8px 16px; border-radius: 20px; font-weight: bold; font-size: 12px; text-transform: uppercase; box-shadow: 0 4px 12px rgba(255, 182, 217, 0.4);">
        ⚡ GIGA
       </div>
       <div class="text-center mb-8">
        <div class="feature-icon text-5xl mb-4">
         💕
        </div>
        <h3 class="font-fredoka text-3xl font-bold" style="color: #E75480;">MILI LOVE CARE</h3>
        <p class="text-sm mt-3 font-medium" style="color: #999;">Suavidade e proteção</p>
        <p class="text-xs mt-2" style="color: #AAA;">Fraldas macias e absorventes para a pele sensível</p>
       </div><!-- Price Section -->
       <div class="mb-8 bg-white rounded-xl p-4"><label class="block text-xs font-bold mb-3 uppercase tracking-wide" style="color: #E75480;">💰 Preço</label>
        <div class="flex items-center gap-3"><span style="color: #E75480; font-weight: bold; font-size: 18px;">R$</span> <input type="number" id="price-mili-love" placeholder="69,99" step="0.01" min="0" class="w-full px-4 py-3 rounded-lg border-2 text-lg font-bold" style="border-color: #FFB6D9; color: #E75480;" value="69.99" oninput="updatePrice(this, 'mili-love')">
        </div>
        <p id="display-price-mili-love" class="text-sm font-bold mt-3 text-center" style="color: #E75480;">R$ 69,99</p>
       </div><!-- Buttons Row -->
       <div class="grid grid-cols-2 gap-3 mb-6"><button class="py-3 rounded-lg text-sm font-bold transition-all hover:scale-105" onclick="openSizeWithPhotos('mili-love')" style="background: linear-gradient(135deg, #FFB6D9, #FF99BB); color: #FFFFFF; border: none; cursor: pointer; box-shadow: 0 4px 12px rgba(255, 182, 217, 0.3);"> 📸 Fotos </button> <button class="py-3 rounded-lg text-sm font-bold transition-all hover:scale-105" onclick="openSizeWithPhotos('mili-love')" style="background: linear-gradient(135deg, #FFB6D9, #FF99BB); color: #FFFFFF; border: none; cursor: pointer; box-shadow: 0 4px 12px rgba(255, 182, 217, 0.3);"> 📏 Tamanhos </button>
       </div><!-- Info Cards -->
       <div class="grid grid-cols-3 gap-2">
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(231, 84, 128, 0.2);">
         <p class="text-2xl mb-1">🛡️</p>
         <p class="text-xs font-bold" style="color: #E75480;">Hipoalergênica</p>
        </div>
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(231, 84, 128, 0.2);">
         <p class="text-2xl mb-1">💧</p>
         <p class="text-xs font-bold" style="color: #E75480;">Absorvente</p>
        </div>
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(231, 84, 128, 0.2);">
         <p class="text-2xl mb-1">�����</p>
         <p class="text-xs font-bold" style="color: #E75480;">Macio</p>
        </div>
       </div>
      </div><!-- Mili Azul Brand -->
      <div class="brand-card animate-slide-in rounded-2xl p-8 shadow-lg" style="background: linear-gradient(135deg, #E8F4F8 0%, #D4EBFF 100%); border: 2px solid #87CEEB; animation-delay: 0.2s;">
       <div class="text-center mb-8">
        <div class="feature-icon text-5xl mb-4">
         💙
        </div>
        <h3 class="font-fredoka text-3xl font-bold" style="color: #0FA3B1;">MILI AZUL</h3>
        <p class="text-sm mt-3 font-medium" style="color: #999;">Conforto e secura</p>
        <p class="text-xs mt-2" style="color: #AAA;">Tecnologia avançada para máximo conforto</p>
       </div><!-- Price Section -->
       <div class="mb-8 bg-white rounded-xl p-4"><label class="block text-xs font-bold mb-3 uppercase tracking-wide" style="color: #0FA3B1;">💰 Preço</label>
        <div class="flex items-center gap-3"><span style="color: #0FA3B1; font-weight: bold; font-size: 18px;">R$</span> <input type="number" id="price-mili-azul" placeholder="0,00" step="0.01" min="0" class="w-full px-4 py-3 rounded-lg border-2 text-lg font-bold" style="border-color: #87CEEB; color: #0FA3B1;" oninput="updatePrice(this, 'mili-azul')">
        </div>
        <p id="display-price-mili-azul" class="text-sm font-bold mt-3 text-center" style="color: #0FA3B1;">Preço não definido</p>
       </div><!-- Gallery Button --> <button onclick="openPhotoGallery('mili-azul')" class="w-full py-4 rounded-xl text-base font-bold transition-all hover:scale-105 mb-6" style="background: linear-gradient(135deg, #87CEEB, #5EC5E0); color: #FFFFFF; border: none; cursor: pointer; box-shadow: 0 4px 12px rgba(135, 206, 235, 0.3);"> 📸 Ver Fotos do Produto </button> <!-- Info Cards -->
       <div class="grid grid-cols-3 gap-2">
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(15, 163, 177, 0.2);">
         <p class="text-2xl mb-1">⏰</p>
         <p class="text-xs font-bold" style="color: #0FA3B1;">12h Proteção</p>
        </div>
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(15, 163, 177, 0.2);">
         <p class="text-2xl mb-1">🎯</p>
         <p class="text-xs font-bold" style="color: #0FA3B1;">Anatômica</p>
        </div>
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(15, 163, 177, 0.2);">
         <p class="text-2xl mb-1">💪</p>
         <p class="text-xs font-bold" style="color: #0FA3B1;">Elástica</p>
        </div>
       </div>
      </div><!-- Pampers Brand -->
      <div class="brand-card animate-slide-in rounded-2xl p-8 shadow-lg" style="background: linear-gradient(135deg, #F0F5FF 0%, #E0E8FF 100%); border: 2px solid #B0C4FF; animation-delay: 0.3s;">
       <div class="text-center mb-8">
        <div class="feature-icon text-5xl mb-4">
         ⭐
        </div>
        <h3 class="font-fredoka text-3xl font-bold" style="color: #5865F2;">PAMPERS</h3>
        <p class="text-sm mt-3 font-medium" style="color: #999;">Premium e confiável</p>
        <p class="text-xs mt-2" style="color: #AAA;">A marca nº 1 recomendada por pediatras</p>
       </div><!-- Price Section -->
       <div class="mb-8 bg-white rounded-xl p-4"><label class="block text-xs font-bold mb-3 uppercase tracking-wide" style="color: #5865F2;">💰 Preço</label>
        <div class="flex items-center gap-3"><span style="color: #5865F2; font-weight: bold; font-size: 18px;">R$</span> <input type="number" id="price-pampers" placeholder="0,00" step="0.01" min="0" class="w-full px-4 py-3 rounded-lg border-2 text-lg font-bold" style="border-color: #B0C4FF; color: #5865F2;" oninput="updatePrice(this, 'pampers')">
        </div>
        <p id="display-price-pampers" class="text-sm font-bold mt-3 text-center" style="color: #5865F2;">Preço não definido</p>
       </div><!-- Gallery Button --> <button onclick="openPhotoGallery('pampers')" class="w-full py-4 rounded-xl text-base font-bold transition-all hover:scale-105 mb-6" style="background: linear-gradient(135deg, #B0C4FF, #8BA1FF); color: #FFFFFF; border: none; cursor: pointer; box-shadow: 0 4px 12px rgba(88, 101, 242, 0.3);"> 📸 Ver Fotos do Produto </button> <!-- Info Cards -->
       <div class="grid grid-cols-3 gap-2">
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(88, 101, 242, 0.2);">
         <p class="text-2xl mb-1">🏆</p>
         <p class="text-xs font-bold" style="color: #5865F2;">Premium</p>
        </div>
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(88, 101, 242, 0.2);">
         <p class="text-2xl mb-1">🧪</p>
         <p class="text-xs font-bold" style="color: #5865F2;">Testada</p>
        </div>
        <div class="bg-white rounded-lg p-3 text-center" style="border: 2px solid rgba(88, 101, 242, 0.2);">
         <p class="text-2xl mb-1">👶</p>
         <p class="text-xs font-bold" style="color: #5865F2;">Suave</p>
        </div>
       </div>
      </div>
     </div><!-- Size Guide Section -->
     <div class="rounded-2xl p-8 mb-12 animate-slide-in" style="background: linear-gradient(135deg, rgba(255,200,221,0.2), rgba(169,208,230,0.2)); border: 2px dashed #AAE4E9; animation-delay: 0.4s;">
      <div class="flex items-center justify-center mb-4"><span class="text-3xl mr-3">📏</span>
       <h3 class="font-fredoka text-2xl font-bold" style="color: #333;">Guia de Tamanhos</h3>
      </div>
      <div class="grid grid-cols-2 md:grid-cols-5 gap-4 text-center">
       <div class="bg-white rounded-lg p-4">
        <p class="font-fredoka font-bold text-lg" style="color: #E75480;">P</p>
        <p class="text-xs mt-2" style="color: #666;">Até 5 kg</p>
       </div>
       <div class="bg-white rounded-lg p-4">
        <p class="font-fredoka font-bold text-lg" style="color: #0FA3B1;">M</p>
        <p class="text-xs mt-2" style="color: #666;">5 - 9 kg</p>
       </div>
       <div class="bg-white rounded-lg p-4">
        <p class="font-fredoka font-bold text-lg" style="color: #5865F2;">G</p>
        <p class="text-xs mt-2" style="color: #666;">9 - 13 kg</p>
       </div>
       <div class="bg-white rounded-lg p-4">
        <p class="font-fredoka font-bold text-lg" style="color: #E75480;">XG</p>
        <p class="text-xs mt-2" style="color: #666;">13 - 18 kg</p>
       </div>
       <div class="bg-white rounded-lg p-4">
        <p class="font-fredoka font-bold text-lg" style="color: #0FA3B1;">XXG+</p>
        <p class="text-xs mt-2" style="color: #666;">Acima de 18 kg</p>
       </div>
      </div>
     </div><!-- Features Section -->
     <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-12">
      <div class="text-center animate-slide-in p-6 rounded-xl" style="background-color: rgba(255,200,221,0.15); animation-delay: 0.5s;">
       <div class="feature-icon">
        🛡️
       </div>
       <h4 class="font-fredoka font-bold text-lg mb-2" style="color: #333;">Proteção</h4>
       <p class="text-sm" style="color: #666;">Proteção contra vazamentos e conforto o dia todo.</p>
      </div>
      <div class="text-center animate-slide-in p-6 rounded-xl" style="background-color: rgba(169,208,230,0.15); animation-delay: 0.6s;">
       <div class="feature-icon">
        😊
       </div>
       <h4 class="font-fredoka font-bold text-lg mb-2" style="color: #333;">Conforto</h4>
       <p class="text-sm" style="color: #666;">Macio e suave para a pele delicada do bebê.</p>
      </div>
      <div class="text-center animate-slide-in p-6 rounded-xl" style="background-color: rgba(88,101,242,0.1); animation-delay: 0.7s;">
       <div class="feature-icon">
        ✅
       </div>
       <h4 class="font-fredoka font-bold text-lg mb-2" style="color: #333;">Qualidade</h4>
       <p class="text-sm" style="color: #666;">Marcas reconhecidas e aprovadas por pediatras.</p>
      </div>
     </div><!-- Call to Action -->
     <div class="rounded-2xl p-8 text-center animate-slide-in mb-8" style="background: linear-gradient(135deg, #87CEEB 0%, #A8D8EA 100%); animation-delay: 0.8s;">
      <h3 class="font-fredoka text-2xl font-bold mb-3" style="color: #FFFFFF;">Pronto para Escolher?</h3>
      <p class="mb-6" style="color: rgba(255,255,255,0.95);">Visite nossa loja e encontre a fralda perfeita para seu bebê. Nossas atendentes estão prontas para ajudar!</p><button id="cta-button" class="px-8 py-3 rounded-lg font-bold text-lg transition-all duration-300 transform hover:scale-105 active:scale-95" style="background-color: #FFFFFF; color: #87CEEB; border: none; cursor: pointer; box-shadow: 0 4px 12px rgba(0,0,0,0.15);"> Entre em Contato �� </button>
     </div>
    </div><!-- Footer -->
    <div class="px-4 py-8 text-center border-t" style="border-color: rgba(135, 206, 235, 0.2); background-color: rgba(255,255,255,0.6);">
     <p id="footer-text" class="text-sm font-medium animate-slide-in" style="color: #666;">Cuidamos do seu bebê como se fosse nosso ��️</p>
     <p class="text-xs mt-2" style="color: #999;">🏥 Farmácia Popular | Qualidade e confiança para sua família</p>
    </div>
   </div>
  </div><!-- Photo Gallery Modal -->
  <div id="photoModal" class="modal-hidden fixed inset-0 z-50 p-4" style="background-color: rgba(0,0,0,0.7); justify-content: center; align-items: center;">
   <div class="bg-white rounded-2xl max-w-2xl w-full max-h-90 overflow-auto shadow-2xl"><!-- Modal Header -->
    <div class="sticky top-0 flex items-center justify-between p-6" style="background: linear-gradient(135deg, #87CEEB, #A8D8EA); z-index: 10;">
     <h3 id="modalTitle" class="font-fredoka text-2xl font-bold" style="color: #FFFFFF;"></h3><button onclick="closePhotoGallery()" class="text-white text-2xl hover:scale-110 transition-transform">×</button>
    </div><!-- Photo Container -->
    <div id="photoContainer" class="p-6"><!-- Photos will be inserted here -->
    </div>
   </div>
  </div><!-- Size Selector Modal -->
  <div id="sizeModal" class="modal-hidden fixed inset-0 z-50 p-4" style="background-color: rgba(0,0,0,0.7); justify-content: center; align-items: center;">
   <div class="bg-white rounded-2xl max-w-2xl w-full max-h-90 overflow-auto shadow-2xl"><!-- Modal Header -->
    <div class="sticky top-0 flex items-center justify-between p-6" style="background: linear-gradient(135deg, #FFB6D9, #FF99BB); z-index: 10;">
     <h3 id="sizeModalTitle" class="font-fredoka text-2xl font-bold" style="color: #FFFFFF;">Tamanhos Disponíveis</h3><button onclick="closeSizeSelector()" class="text-white text-2xl hover:scale-110 transition-transform">×</button>
    </div><!-- Size Container -->
    <div id="sizeContainer" class="p-6"><!-- Sizes will be inserted here -->
    </div>
   </div>
  </div>
  <script>
    const defaultConfig = {
      catalog_title: 'Catálogo de Fraldas',
      subtitle_text: 'Escolha o tamanho ideal para seu bebê',
      footer_text: 'Cuidamos do seu bebê como se fosse nosso ❤️',
      primary_color: '#87CEEB',
      secondary_color: '#A8D8EA',
      text_color: '#333333',
      accent_color: '#FFFFFF',
      font_family: 'Fredoka',
      font_size: 16
    };

    // Photo Gallery Data
    const photoGalleries = {
      'mili-love': {
        title: '💕 MILI LOVE CARE - Fotos do Produto',
        photos: [
          {
            image: 'https://m.media-amazon.com/images/I/71fJDr5F7FL._AC_UF1000,1000_QL80_.jpg',
            description: 'Mili Love Care - Embalagem frente'
          },
          {
            image: 'https://m.media-amazon.com/images/I/71v3p5aFWjL._AC_UF1000,1000_QL80_.jpg',
            description: 'Mili Love Care - Proteção e conforto'
          },
          {
            image: 'https://m.media-amazon.com/images/I/71fJDr5F7FL._AC_UF1000,1000_QL80_.jpg',
            description: 'Mili Love Care - Vista lateral'
          }
        ]
      },
      'mili-azul': {
        title: '💙 MILI AZUL - Fotos do Produto',
        photos: [
          {
            image: 'https://m.media-amazon.com/images/I/71xvNt47ZzL._AC_UF1000,1000_QL80_.jpg',
            description: 'Mili Azul - Embalagem frente'
          },
          {
            image: 'https://m.media-amazon.com/images/I/71xvNt47ZzL._AC_UF1000,1000_QL80_.jpg',
            description: 'Mili Azul - Design moderno'
          },
          {
            image: 'https://m.media-amazon.com/images/I/71xvNt47ZzL._AC_UF1000,1000_QL80_.jpg',
            description: 'Mili Azul - Qualidade premium'
          }
        ]
      },
      'pampers': {
        title: '⭐ PAMPERS - Fotos do Produto',
        photos: [
          {
            image: 'https://m.media-amazon.com/images/I/71Z+5Lx-7OL._AC_UF1000,1000_QL80_.jpg',
            description: 'Pampers Swaddlers - Embalagem'
          },
          {
            image: 'https://m.media-amazon.com/images/I/71Z+5Lx-7OL._AC_UF1000,1000_QL80_.jpg',
            description: 'Pampers - Proteção Premium'
          },
          {
            image: 'https://m.media-amazon.com/images/I/71Z+5Lx-7OL._AC_UF1000,1000_QL80_.jpg',
            description: 'Pampers - Número 1 do mercado'
          }
        ]
      }
    };

    // Size Data
    const sizeData = {
      'mili-love': {
        title: '💕 MILI LOVE CARE - Tamanhos',
        sizes: ['P', 'M', 'G', 'XG', 'XXG'],
        color: '#E75480'
      },
      'mili-azul': {
        title: '💙 MILI AZUL - Tamanhos',
        sizes: ['P', 'M', 'G', 'XG', 'XXG'],
        color: '#0FA3B1'
      },
      'pampers': {
        title: '⭐ PAMPERS - Tamanhos',
        sizes: ['P', 'M', 'G', 'XG', 'XXG', 'XXXG'],
        color: '#5865F2'
      }
    };

    const sizeInfo = {
      'P': { label: 'P', weight: 'Até 5 kg', emoji: '👶' },
      'M': { label: 'M', weight: '5 - 9 kg', emoji: '👧' },
      'G': { label: 'G', weight: '9 - 13 kg', emoji: '🧒' },
      'XG': { label: 'XG', weight: '13 - 18 kg', emoji: '👦' },
      'XXG': { label: 'XXG', weight: 'Acima de 18 kg', emoji: '🧑' },
      'XXXG': { label: 'XXXG', weight: 'Acima de 18 kg', emoji: '🧑' }
    };

    function openPhotoGallery(galleryId) {
      const gallery = photoGalleries[galleryId];
      if (!gallery) return;

      const modal = document.getElementById('photoModal');
      const container = document.getElementById('photoContainer');
      const title = document.getElementById('modalTitle');

      title.textContent = gallery.title;
      container.innerHTML = '';

      // Create photo grid
      const grid = document.createElement('div');
      grid.className = 'photo-grid';

      gallery.photos.forEach((photo, index) => {
        const photoDiv = document.createElement('div');
        photoDiv.className = 'photo-item';
        photoDiv.style.backgroundColor = '#F5F5F5';

        const img = document.createElement('img');
        img.src = photo.image;
        img.loading = 'lazy';
        img.alt = photo.description;
        img.onerror = function() {
          console.error('Imagem não carregou:', photo.image);
          this.parentElement.style.backgroundColor = '#E0E0E0';
          this.alt = 'Imagem indisponível';
        };

        photoDiv.appendChild(img);

        const desc = document.createElement('div');
        desc.style.cssText = `
          padding: 8px;
          font-size: 12px;
          font-weight: 600;
          text-align: center;
          background-color: #F5F5F5;
          color: #666;
        `;
        desc.textContent = photo.description;

        photoDiv.appendChild(desc);
        grid.appendChild(photoDiv);
      });

      container.appendChild(grid);
      modal.classList.remove('modal-hidden');
      modal.classList.add('modal-visible');
    }

    function closePhotoGallery() {
      const modal = document.getElementById('photoModal');
      modal.classList.add('modal-hidden');
      modal.classList.remove('modal-visible');
    }

    function openSizeSelector(brandId) {
      const sizeInfo_ = sizeData[brandId];
      if (!sizeInfo_) return;

      const modal = document.getElementById('sizeModal');
      const container = document.getElementById('sizeContainer');
      const title = document.getElementById('sizeModalTitle');

      title.textContent = sizeInfo_.title;
      title.style.color = '#FFFFFF';

      // Update modal header color
      const modalHeader = modal.querySelector('[style*="background"]');
      const header = modal.querySelector('.sticky');
      if (header) {
        header.style.background = `linear-gradient(135deg, ${sizeInfo_.color}, ${sizeInfo_.color}dd)`;
      }

      container.innerHTML = '';

      // Create size grid
      const grid = document.createElement('div');
      grid.style.display = 'grid';
      grid.style.gridTemplateColumns = 'repeat(auto-fit, minmax(120px, 1fr))';
      grid.style.gap = '12px';

      sizeInfo_.sizes.forEach(size => {
        const sizeCard = document.createElement('div');
        sizeCard.style.cssText = `
          background: linear-gradient(135deg, ${sizeInfo_.color}15, ${sizeInfo_.color}08);
          border: 2px solid ${sizeInfo_.color};
          border-radius: 16px;
          padding: 20px;
          text-align: center;
          cursor: pointer;
          transition: all 0.3s ease;
        `;

        const info = sizeInfo[size];
        sizeCard.innerHTML = `
          <div style="font-size: 32px; margin-bottom: 8px;">${info.emoji}</div>
          <div style="font-size: 24px; font-weight: bold; color: ${sizeInfo_.color}; margin-bottom: 6px;">${info.label}</div>
          <div style="font-size: 12px; color: #666; font-weight: 600;">${info.weight}</div>
        `;

        sizeCard.addEventListener('mouseenter', function() {
          this.style.transform = 'scale(1.1)';
          this.style.boxShadow = `0 8px 24px rgba(0,0,0,0.15)`;
        });

        sizeCard.addEventListener('mouseleave', function() {
          this.style.transform = 'scale(1)';
          this.style.boxShadow = 'none';
        });

        grid.appendChild(sizeCard);
      });

      container.appendChild(grid);
      modal.classList.remove('modal-hidden');
      modal.classList.add('modal-visible');
    }

    function closeSizeSelector() {
      const modal = document.getElementById('sizeModal');
      modal.classList.add('modal-hidden');
      modal.classList.remove('modal-visible');
    }

    function openSizeWithPhotos(brandId) {
      const sizeInfo_ = sizeData[brandId];
      const gallery = photoGalleries[brandId];
      if (!sizeInfo_ || !gallery) return;

      const modal = document.getElementById('sizeModal');
      const container = document.getElementById('sizeContainer');
      const title = document.getElementById('sizeModalTitle');

      title.textContent = sizeInfo_.title;
      title.style.color = '#FFFFFF';

      // Update modal header color
      const header = modal.querySelector('.sticky');
      if (header) {
        header.style.background = `linear-gradient(135deg, ${sizeInfo_.color}, ${sizeInfo_.color}dd)`;
      }

      container.innerHTML = '';

      // Create main wrapper
      const wrapper = document.createElement('div');
      wrapper.style.cssText = 'display: flex; flex-direction: column; gap: 24px;';

      // Create size grid
      const grid = document.createElement('div');
      grid.style.display = 'grid';
      grid.style.gridTemplateColumns = 'repeat(auto-fit, minmax(100px, 1fr))';
      grid.style.gap = '12px';

      sizeInfo_.sizes.forEach(size => {
        const sizeCard = document.createElement('div');
        sizeCard.style.cssText = `
          background: linear-gradient(135deg, ${sizeInfo_.color}15, ${sizeInfo_.color}08);
          border: 2px solid ${sizeInfo_.color};
          border-radius: 16px;
          padding: 16px;
          text-align: center;
          cursor: pointer;
          transition: all 0.3s ease;
        `;

        const info = sizeInfo[size];
        sizeCard.innerHTML = `
          <div style="font-size: 28px; margin-bottom: 6px;">${info.emoji}</div>
          <div style="font-size: 20px; font-weight: bold; color: ${sizeInfo_.color}; margin-bottom: 4px;">${info.label}</div>
          <div style="font-size: 11px; color: #666; font-weight: 600;">${info.weight}</div>
        `;

        sizeCard.addEventListener('mouseenter', function() {
          this.style.transform = 'scale(1.1)';
          this.style.boxShadow = `0 8px 24px rgba(0,0,0,0.15)`;
        });

        sizeCard.addEventListener('mouseleave', function() {
          this.style.transform = 'scale(1)';
          this.style.boxShadow = 'none';
        });

        grid.appendChild(sizeCard);
      });

      wrapper.appendChild(grid);

      // Add divider
      const divider = document.createElement('div');
      divider.style.cssText = 'height: 2px; background: linear-gradient(90deg, transparent, #ddd, transparent); margin: 12px 0;';
      wrapper.appendChild(divider);

      // Create photos section
      const photosTitle = document.createElement('h4');
      photosTitle.textContent = '📸 Fotos do Produto';
      photosTitle.style.cssText = `font-weight: bold; color: ${sizeInfo_.color}; margin: 8px 0; font-size: 14px;`;
      wrapper.appendChild(photosTitle);

      // Create photo grid
      const photoGrid = document.createElement('div');
      photoGrid.className = 'photo-grid';

      gallery.photos.forEach((photo, index) => {
        const photoDiv = document.createElement('div');
        photoDiv.className = 'photo-item';
        photoDiv.style.backgroundColor = '#F5F5F5';

        const img = document.createElement('img');
        img.src = photo.image;
        img.loading = 'lazy';
        img.alt = photo.description;
        img.onerror = function() {
          console.error('Imagem não carregou:', photo.image);
          this.parentElement.style.backgroundColor = '#E0E0E0';
          this.alt = 'Imagem indisponível';
        };

        photoDiv.appendChild(img);

        const desc = document.createElement('div');
        desc.style.cssText = `
          padding: 8px;
          font-size: 11px;
          font-weight: 600;
          text-align: center;
          background-color: #F5F5F5;
          color: #666;
        `;
        desc.textContent = photo.description;

        photoDiv.appendChild(desc);
        photoGrid.appendChild(photoDiv);
      });

      wrapper.appendChild(photoGrid);
      container.appendChild(wrapper);
      modal.classList.remove('modal-hidden');
      modal.classList.add('modal-visible');
    }

    // Close modals when clicking outside
    document.getElementById('photoModal').addEventListener('click', (e) => {
      if (e.target.id === 'photoModal') {
        closePhotoGallery();
      }
    });

    document.getElementById('sizeModal').addEventListener('click', (e) => {
      if (e.target.id === 'sizeModal') {
        closeSizeSelector();
      }
    });

    // Price update function
    function updatePrice(input, brand) {
      const price = parseFloat(input.value);
      const displayElement = document.getElementById(`display-price-${brand}`);
      
      if (input.value === '' || isNaN(price)) {
        displayElement.textContent = 'Preço não definido';
      } else {
        displayElement.textContent = `R$ ${price.toFixed(2).replace('.', ',')}`;
      }
    }

    // Size photo handler
    function handleSizePhoto(input) {
      const file = input.files[0];
      if (!file) return;

      const brand = input.getAttribute('data-brand');
      const size = input.getAttribute('data-size');
      const previewId = `preview-${brand}-${size}`;
      const previewDiv = document.getElementById(previewId);

      if (file.type.startsWith('image/')) {
        const reader = new FileReader();
        reader.onload = function(e) {
          const img = previewDiv.querySelector('img');
          img.src = e.target.result;
          previewDiv.style.display = 'block';
        };
        reader.readAsDataURL(file);
      }
    }

    // Size selection functionality
    document.querySelectorAll('.size-button').forEach(button => {
      button.addEventListener('click', function() {
        const brand = this.getAttribute('data-brand');
        const allButtons = document.querySelectorAll(`[data-brand="${brand}"]`);
        
        allButtons.forEach(btn => {
          btn.classList.remove('active');
          btn.style.backgroundColor = '#F5F5F5';
          btn.style.color = '#666';
        });
        
        this.classList.add('active');
        this.style.backgroundColor = this.style.borderColor || '#87CEEB';
        this.style.color = '#FFFFFF';
      });
    });

    // CTA Button interaction
    document.getElementById('cta-button').addEventListener('click', function() {
      const feedback = document.createElement('div');
      feedback.style.cssText = `
        position: fixed;
        bottom: 20px;
        left: 50%;
        transform: translateX(-50%);
        background-color: #87CEEB;
        color: white;
        padding: 14px 28px;
        border-radius: 12px;
        font-weight: 600;
        font-size: 14px;
        animation: slide-in 0.3s ease-out;
        box-shadow: 0 4px 12px rgba(135, 206, 235, 0.3);
        z-index: 100;
      `;
      feedback.textContent = '✓ Obrigado pelo interesse! Entraremos em contato em breve.';
      document.body.appendChild(feedback);
      
      setTimeout(() => {
        feedback.style.animation = 'slide-in 0.3s ease-out reverse';
        setTimeout(() => feedback.remove(), 300);
      }, 3000);
    });

    async function onConfigChange(config) {
      document.getElementById('catalog-title').textContent = config.catalog_title || defaultConfig.catalog_title;
      document.getElementById('subtitle-text').textContent = config.subtitle_text || defaultConfig.subtitle_text;
      document.getElementById('footer-text').textContent = config.footer_text || defaultConfig.footer_text;

      const customFont = config.font_family || defaultConfig.font_family;
      document.body.style.fontFamily = `${customFont}, sans-serif`;

      const baseSize = config.font_size || defaultConfig.font_size;
    }

    function mapToCapabilities(config) {
      return {
        recolorables: [
          {
            get: () => config.primary_color || defaultConfig.primary_color,
            set: (value) => {
              config.primary_color = value;
              window.elementSdk.setConfig({ primary_color: value });
            }
          },
          {
            get: () => config.secondary_color || defaultConfig.secondary_color,
            set: (value) => {
              config.secondary_color = value;
              window.elementSdk.setConfig({ secondary_color: value });
            }
          }
        ],
        borderables: [],
        fontEditable: {
          get: () => config.font_family || defaultConfig.font_family,
          set: (value) => {
            config.font_family = value;
            window.elementSdk.setConfig({ font_family: value });
          }
        },
        fontSizeable: {
          get: () => config.font_size || defaultConfig.font_size,
          set: (value) => {
            config.font_size = value;
            window.elementSdk.setConfig({ font_size: value });
          }
        }
      };
    }

    function mapToEditPanelValues(config) {
      return new Map([
        ['catalog_title', config.catalog_title || defaultConfig.catalog_title],
        ['subtitle_text', config.subtitle_text || defaultConfig.subtitle_text],
        ['footer_text', config.footer_text || defaultConfig.footer_text]
      ]);
    }

    if (window.elementSdk) {
      window.elementSdk.init({
        defaultConfig,
        onConfigChange,
        mapToCapabilities,
        mapToEditPanelValues
      });
    }
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9c8d13d9d447f1ce',t:'MTc3MDIzODYxNi4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
