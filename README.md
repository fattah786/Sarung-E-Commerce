<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Toko Sarung Bang Doel - Sarung Asli Bandung</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=DM+Serif+Display&family=Great+Vibes&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Toko Sarung Bang Doel</h1>
        <div class="cart-icon" onclick="toggleCart()">
            🛒
            <span class="cart-count" id="cartCount">0</span>
        </div>
    </header>
    
    <nav>
        <ul>
            <li><a href="#beranda">Beranda</a></li>
            <li><a href="#produk">Produk</a></li>
            <li><a href="#kategori">Kategori</a></li>
            <li><a href="#tentang">Tentang Kami</a></li>
            <li><a href="#kontak">Kontak</a></li>
        </ul>
    </nav>
    
    <main>
        <section id="beranda" class="hero">
            <h2>Selamat Datang di Toko Sarung Bang Doel</h2>
            <p>Koleksi sarung tradisional dan modern terbaik dari Bandung dengan kualitas premium dan harga terjangkau</p>
        </section>
        
        <section id="kategori">
            <h2 class="section-title">Kategori Produk</h2>
            <div class="categories">
                <a href="#" class="category">
                    <h3>Sarung Batik</h3>
                    <p>Motif tradisional dan modern</p>
                </a>
                <a href="#" class="category">
                    <h3>Sarung Tenun</h3>
                    <p>Tenun ikat berkualitas tinggi</p>
                </a>
                <a href="#" class="category">
                    <h3>Sarung Songket</h3>
                    <p>Mewah dengan benang emas</p>
                </a>
                <a href="#" class="category">
                    <h3>Sarung Modern</h3>
                    <p>Desain kontemporer</p>
                </a>
            </div>
        </section>
        
        <section id="produk">
            <h2 class="section-title">Produk Terbaru</h2>
            <div class="products">
                <article class="product">
                    <img src="Wayang.jpg" alt="Sarung Batik Tradisional">
                    <div class="product-info">
                        <h3>Sarung Batik Tradisional Bandung</h3>
                        <p>Sarung batik dengan motif tradisional dan motif wayang, dibuat dengan teknik canting tulis asli Bandung. Bahan katun premium yang nyaman dan tahan lama.</p>
                        <div class="price">Rp 350.000</div>
                        <button class="buy-btn" onclick="addToCart(1, 'Sarung Batik Tradisional Bandung', 350000)">Beli Sekarang</button>
                    </div>
                </article>
                
                <article class="product">
                    <img src="Modern.jpg" alt="Sarung Tenun Ikat">
                    <div class="product-info">
                        <h3>Sarung Tenun Ikat Bandung</h3>
                        <p>Sarung tenun khas Nusa Tenggara, ditenun manual dengan benang katun pilihan terbaik. Motif etnik yang memukau dan bernilai seni tinggi.</p>
                        <div class="price">Rp 450.000</div>
                        <button class="buy-btn" onclick="addToCart(2, 'Sarung Tenun Ikat Bandung', 450000)">Beli Sekarang</button>
                    </div>
                </article>
                
                <article class="product">
                    <img src="Songket.jpg" alt="Sarung Songket Mewah">
                    <div class="product-info">
                        <h3>Sarung Songket Bandung</h3>
                        <p>Sarung songket mewah dengan benang emas asli, cocok untuk acara resmi dan pernikahan. Keanggunan tradisional yang tak lekang waktu.</p>
                        <div class="price">Rp 1.250.000</div>
                        <button class="buy-btn" onclick="addToCart(3, 'Sarung Songket Bandung', 1250000)">Beli Sekarang</button>
                    </div>
                </article>
                
                <article class="product">
                    <img src="Tenun Batik.jpg" alt="Sarung Batik Modern Bandung">
                    <div class="product-info">
                        <h3>Sarung Batik Modern</h3>
                        <p>Sarung batik dengan motif kontemporer, nyaman dipakai sehari-hari. Perpaduan sempurna antara tradisi dan modernitas.</p>
                        <div class="price">Rp 180.000</div>
                        <button class="buy-btn" onclick="addToCart(4, 'Sarung Batik Modern', 180000)">Beli Sekarang</button>
                    </div>
                </article>
                
                <article class="product">
                    <img src="Sutra.jpeg" alt="Sarung Sutera Premium Bandung">
                    <div class="product-info">
                        <h3>Sarung Sutera Premium</h3>
                        <p>Sarung berbahan sutera halus dengan motif eksklusif. Kemewahan dan kenyamanan dalam satu produk berkualitas tinggi.</p>
                        <div class="price">Rp 750.000</div>
                        <button class="buy-btn" onclick="addToCart(5, 'Sarung Sutera Premium', 750000)">Beli Sekarang</button>
                    </div>
                </article>
            </div>
        </section>
        
        <section id="tentang" class="about">
            <h3>Tentang Kami</h3>
            <p>Toko Sarung Bang Doel telah berdiri sejak 2000 dan menjadi toko sarung terpercaya di Bandung. Kami menyediakan berbagai jenis sarung berkualitas tinggi dari berbagai daerah di Indonesia. Dengan pengalaman lebih dari 25 tahun, kami berkomitmen memberikan produk terbaik dengan harga yang kompetitif untuk semua kalangan.</p>
        </section>
    </main>
    
    <!-- Cart Modal -->
    <div id="cartModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeCart()">&times;</span>
            <h2>Keranjang Belanja</h2>
            <div id="cartItems"></div>
            <div class="cart-total" id="cartTotal">Total: Rp 0</div>
            <button class="checkout-btn" onclick="checkout()">Checkout</button>
        </div>
    </div>
    
    <!-- Notification -->
    <div id="notification" class="notification"></div>
    
    <footer id="kontak">
        <div class="footer-content">
            <div class="footer-section">
                <h4>Kontak Kami</h4>
                <p>📍 Jl. H. Djuanda Kec. Cicalengka Kab. Bandung<br>
                📞 (089) 5364530205<br>
                📧 info@sarungbangdoel.com</p>
            </div>
            <div class="footer-section">
                <h4>Jam Operasional</h4>
                <p>Senin - Sabtu: 08:00 - 16:00<br>
                Minggu: 10:00 - 16:00</p>
            </div>
            <div class="footer-section">
                <h4>Media Sosial</h4>
                <p>
                    <a href="#">Facebook tokosarungbangdoel</a><br>
                    <a href="#">Instagram tokosarungbangdoel</a><br>
                    <a href="#">WhatsApp (0895364530205)</a>
                </p>
            </div>
        </div>
        <hr style="margin: 2rem 0; border: 1px solid #34495e;">
        <p>&copy; 2025 Toko Sarung Bang Doel. Seluruh hak cipta dilindungi.</p>
    </footer>

    <script>
        let cart = [];
        let cartCount = 0;

        function addToCart(id, name, price) {
            const existingItem = cart.find(item => item.id === id);
            
            if (existingItem) {
                existingItem.quantity += 1;
            } else {
                cart.push({ id, name, price, quantity: 1 });
            }
            
            cartCount++;
            updateCartDisplay();
            showNotification(`${name} ditambahkan ke keranjang!`);
        }

        function removeFromCart(id) {
            const itemIndex = cart.findIndex(item => item.id === id);
            if (itemIndex !== -1) {
                cartCount -= cart[itemIndex].quantity;
                cart.splice(itemIndex, 1);
                updateCartDisplay();
                showNotification('Produk dihapus dari keranjang');
            }
        }

        function updateQuantity(id, change) {
            const item = cart.find(item => item.id === id);
            if (item) {
                item.quantity += change;
                if (item.quantity <= 0) {
                    removeFromCart(id);
                } else {
                    cartCount += change;
                    updateCartDisplay();
                }
            }
        }

        function updateCartDisplay() {
            document.getElementById('cartCount').textContent = cartCount;
            const cartItems = document.getElementById('cartItems');
            const cartTotal = document.getElementById('cartTotal');
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<div class="empty-cart">Keranjang belanja kosong</div>';
                cartTotal.textContent = 'Total: Rp 0';
            } else {
                let total = 0;
                cartItems.innerHTML = cart.map(item => {
                    const itemTotal = item.price * item.quantity;
                    total += itemTotal;
                    return `
                        <div class="cart-item">
                            <div class="cart-item-info">
                                <div class="cart-item-title">${item.name}</div>
                                <div class="cart-item-price">Rp ${item.price.toLocaleString()}</div>
                            </div>
                            <div class="quantity-controls">
                                <button class="quantity-btn" onclick="updateQuantity(${item.id}, -1)">-</button>
                                <span class="quantity">${item.quantity}</span>
                                <button class="quantity-btn" onclick="updateQuantity(${item.id}, 1)">+</button>
                            </div>
                            <button class="remove-btn" onclick="removeFromCart(${item.id})">Hapus</button>
                        </div>
                    `;
                }).join('');
                cartTotal.textContent = `Total: Rp ${total.toLocaleString()}`;
            }
        }

        function toggleCart() {
            document.getElementById('cartModal').style.display = 'block';
        }

        function closeCart() {
            document.getElementById('cartModal').style.display = 'none';
        }

        function checkout() {
            if (cart.length === 0) {
                alert('Keranjang belanja kosong!');
                return;
            }
            
            const total = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            const message = `Halo, saya ingin memesan:\n\n${cart.map(item => `${item.name} x${item.quantity} = Rp ${(item.price * item.quantity).toLocaleString()}`).join('\n')}\n\nTotal: Rp ${total.toLocaleString()}`;
            const whatsappUrl = `https://wa.me/6289536453025?text=${encodeURIComponent(message)}`;
            window.open(whatsappUrl, '_blank');
        }

        function showNotification(message) {
            const notification = document.getElementById('notification');
            notification.textContent = message;
            notification.classList.add('show');
            setTimeout(() => {
                notification.classList.remove('show');
            }, 3000);
        }
    </script>
</body>
</html>
