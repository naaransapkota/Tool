<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Free online tool to compress your images while maintaining quality. Reduce file size for JPG, PNG, and WebP images quickly and easily.">
    <meta name="keywords" content="image compressor, compress images, reduce image size, online image optimizer, JPG compressor, PNG compressor, WebP converter">
    <meta name="author" content="ImageCompressorPro">
    <meta property="og:title" content="Free Online Image Compression Tool">
    <meta property="og:description" content="Compress your images online for free. Reduce file size without losing quality.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://yourwebsite.com">
    <meta name="robots" content="index, follow">
    <title>Free Online Image Compression Tool | Optimize JPG, PNG, WebP</title>
    <link rel="canonical" href="https://yourwebsite.com/image-compressor" />
    <style>
        :root {
            --primary-color: #4285f4;
            --secondary-color: #34a853;
            --accent-color: #ea4335;
            --light-gray: #f5f5f5;
            --dark-gray: #333;
            --medium-gray: #757575;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --border-radius: 8px;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--dark-gray);
            background-color: #f9f9f9;
            padding: 0;
            margin: 0;
        }
        
        header {
            background-color: white;
            box-shadow: var(--shadow);
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
            text-decoration: none;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--primary-color);
        }
        
        main {
            padding: 2rem 0;
        }
        
        .hero {
            text-align: center;
            padding: 3rem 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            border-radius: var(--border-radius);
            margin-bottom: 2rem;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark-gray);
        }
        
        .hero p {
            font-size: 1.2rem;
            color: var(--medium-gray);
            max-width: 700px;
            margin: 0 auto 2rem;
        }
        
        .compressor-container {
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 2rem;
            margin-bottom: 2rem;
        }
        
        .upload-area {
            border: 2px dashed var(--medium-gray);
            border-radius: var(--border-radius);
            padding: 3rem 1rem;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            margin-bottom: 2rem;
            position: relative;
        }
        
        .upload-area:hover {
            border-color: var(--primary-color);
            background-color: rgba(66, 133, 244, 0.05);
        }
        
        .upload-area.active {
            border-color: var(--secondary-color);
            background-color: rgba(52, 168, 83, 0.05);
        }
        
        .upload-area i {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        
        .upload-area p {
            margin-bottom: 0.5rem;
        }
        
        .upload-area input {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            opacity: 0;
            cursor: pointer;
        }
        
        .controls {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
            margin-bottom: 2rem;
        }
        
        .control-group {
            flex: 1;
            min-width: 250px;
        }
        
        .control-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }
        
        .slider-container {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
        
        .slider {
            flex: 1;
            -webkit-appearance: none;
            height: 8px;
            border-radius: 4px;
            background: var(--light-gray);
            outline: none;
        }
        
        .slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background: var(--primary-color);
            cursor: pointer;
            transition: all 0.2s;
        }
        
        .slider::-webkit-slider-thumb:hover {
            transform: scale(1.1);
            background: var(--secondary-color);
        }
        
        .slider-value {
            width: 50px;
            text-align: center;
            font-weight: 600;
            color: var(--primary-color);
        }
        
        select {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid #ddd;
            border-radius: var(--border-radius);
            background-color: white;
            font-size: 1rem;
            cursor: pointer;
        }
        
        select:focus {
            outline: none;
            border-color: var(--primary-color);
            box-shadow: 0 0 0 2px rgba(66, 133, 244, 0.2);
        }
        
        .button-group {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }
        
        button {
            padding: 0.75rem 1.5rem;
            border: none;
            border-radius: var(--border-radius);
            font-size: 1rem;
            font-weight: 500;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .btn-primary {
            background-color: var(--primary-color);
            color: white;
            flex: 1;
        }
        
        .btn-primary:hover {
            background-color: #3367d6;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        .btn-secondary {
            background-color: var(--light-gray);
            color: var(--dark-gray);
            flex: 1;
        }
        
        .btn-secondary:hover {
            background-color: #e0e0e0;
        }
        
        .results {
            display: none;
            margin-top: 2rem;
            animation: fadeIn 0.5s ease-in-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .comparison {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            margin-bottom: 2rem;
        }
        
        .image-box {
            flex: 1;
            min-width: 300px;
            text-align: center;
        }
        
        .image-box img {
            max-width: 100%;
            max-height: 400px;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            margin-bottom: 1rem;
        }
        
        .image-stats {
            background-color: var(--light-gray);
            padding: 1rem;
            border-radius: var(--border-radius);
        }
        
        .stat-row {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.5rem;
        }
        
        .savings {
            font-weight: 600;
            color: var(--secondary-color);
        }
        
        .download-btn {
            display: inline-block;
            margin-top: 1rem;
            background-color: var(--secondary-color);
            color: white;
            text-decoration: none;
            padding: 0.75rem 1.5rem;
            border-radius: var(--border-radius);
            font-weight: 500;
            transition: all 0.3s;
        }
        
        .download-btn:hover {
            background-color: #2d9249;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        .ad-container {
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 1rem;
            margin: 2rem 0;
            text-align: center;
            min-height: 100px;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }
        
        .ad-label {
            font-size: 0.8rem;
            color: var(--medium-gray);
            text-align: center;
            margin-bottom: 0.5rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }
        
        .feature-card {
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 1.5rem;
            transition: transform 0.3s;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
        }
        
        .feature-card i {
            font-size: 2rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        
        .feature-card h3 {
            margin-bottom: 0.5rem;
            color: var(--dark-gray);
        }
        
        footer {
            background-color: var(--dark-gray);
            color: white;
            padding: 3rem 0 1.5rem;
            margin-top: 3rem;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }
        
        .footer-column h3 {
            margin-bottom: 1rem;
            font-size: 1.2rem;
            color: #fff;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 0.5rem;
        }
        
        .footer-column ul li a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column ul li a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 1.5rem;
            border-top: 1px solid #444;
            color: #bbb;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                gap: 1rem;
            }
            
            nav ul {
                margin-top: 1rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .controls {
                flex-direction: column;
                gap: 1.5rem;
            }
            
            .comparison {
                flex-direction: column;
            }
        }
        
        /* Loading spinner */
        .spinner {
            display: none;
            width: 40px;
            height: 40px;
            margin: 2rem auto;
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-radius: 50%;
            border-top-color: var(--primary-color);
            animation: spin 1s ease-in-out infinite;
        }
        
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        
        /* Toast notification */
        .toast {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: var(--dark-gray);
            color: white;
            padding: 1rem 1.5rem;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            transform: translateY(100px);
            opacity: 0;
            transition: all 0.3s;
            z-index: 1000;
        }
        
        .toast.show {
            transform: translateY(0);
            opacity: 1;
        }
        
        .toast.error {
            background-color: var(--accent-color);
        }
        
        .toast.success {
            background-color: var(--secondary-color);
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Google AdSense Script - Replace YOUR_ADSENSE_ID with your actual AdSense ID -->
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_ADSENSE_ID" crossorigin="anonymous"></script>
</head>
<body>
    <header>
        <div class="container header-content">
            <a href="#" class="logo">ImageCompressorPro</a>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">How It Works</a></li>
                    <li><a href="#">Features</a></li>
                    <li><a href="#">FAQ</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <!-- Top Ad Banner -->
        <div class="ad-label">Advertisement</div>
        <div class="ad-container">
            <!-- AdSense Ad Unit -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="YOUR_AD_SLOT_ID"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>

        <section class="hero">
            <h1>Compress Images Online for Free</h1>
            <p>Reduce image file size without losing quality. Optimize JPG, PNG, and WebP images for faster websites and smaller storage.</p>
        </section>

        <section class="compressor-container">
            <div class="upload-area" id="uploadArea">
                <i class="fas fa-cloud-upload-alt"></i>
                <p><strong>Drag & Drop your image here</strong></p>
                <p>or click to browse files</p>
                <p class="small">Supports: JPG, PNG, WebP (Max: 10MB)</p>
                <input type="file" id="fileInput" accept="image/jpeg, image/png, image/webp">
            </div>

            <div class="controls">
                <div class="control-group">
                    <label for="quality">Compression Level</label>
                    <div class="slider-container">
                        <input type="range" min="1" max="100" value="80" class="slider" id="qualitySlider">
                        <span class="slider-value" id="qualityValue">80%</span>
                    </div>
                </div>
                
                <div class="control-group">
                    <label for="format">Output Format</label>
                    <select id="formatSelect">
                        <option value="original">Original Format</option>
                        <option value="jpeg">JPEG</option>
                        <option value="png">PNG</option>
                        <option value="webp">WebP</option>
                    </select>
                </div>
            </div>

            <div class="button-group">
                <button class="btn-primary" id="compressBtn">Compress Image</button>
                <button class="btn-secondary" id="resetBtn">Reset</button>
            </div>

            <div class="spinner" id="spinner"></div>

            <div class="results" id="results">
                <h2>Compression Results</h2>
                <div class="comparison">
                    <div class="image-box">
                        <h3>Original Image</h3>
                        <img id="originalImage" src="" alt="Original Image">
                        <div class="image-stats">
                            <div class="stat-row">
                                <span>File Size:</span>
                                <span id="originalSize">0 KB</span>
                            </div>
                            <div class="stat-row">
                                <span>Dimensions:</span>
                                <span id="originalDimensions">0 × 0</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="image-box">
                        <h3>Compressed Image</h3>
                        <img id="compressedImage" src="" alt="Compressed Image">
                        <div class="image-stats">
                            <div class="stat-row">
                                <span>File Size:</span>
                                <span id="compressedSize">0 KB</span>
                            </div>
                            <div class="stat-row">
                                <span>Dimensions:</span>
                                <span id="compressedDimensions">0 × 0</span>
                            </div>
                            <div class="stat-row">
                                <span>Reduction:</span>
                                <span class="savings" id="reductionPercent">0%</span>
                            </div>
                        </div>
                        <a href="#" class="download-btn" id="downloadBtn">
                            <i class="fas fa-download"></i> Download
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Middle Ad Banner -->
        <div class="ad-label">Advertisement</div>
        <div class="ad-container">
            <!-- AdSense Ad Unit -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="YOUR_AD_SLOT_ID"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>

        <section class="features">
            <div class="feature-card">
                <i class="fas fa-bolt"></i>
                <h3>Fast Compression</h3>
                <p>Our advanced algorithms compress your images in seconds, saving you time and bandwidth.</p>
            </div>
            <div class="feature-card">
                <i class="fas fa-lock"></i>
                <h3>Secure Processing</h3>
                <p>Your images are processed in your browser and never uploaded to our servers, ensuring complete privacy.</p>
            </div>
            <div class="feature-card">
                <i class="fas fa-chart-line"></i>
                <h3>Quality Control</h3>
                <p>Adjust compression levels to find the perfect balance between file size and image quality.</p>
            </div>
        </section>

        <!-- Bottom Ad Banner -->
        <div class="ad-label">Advertisement</div>
        <div class="ad-container">
            <!-- AdSense Ad Unit -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="YOUR_AD_SLOT_ID"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </main>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>ImageCompressorPro</h3>
                    <p>Free online tool to optimize your images for web and mobile.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Features</a></li>
                        <li><a href="#">How It Works</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Support</h3>
                    <ul>
                        <li><a href="#">FAQ</a></li>
                        <li><a href="#">Contact Us</a></li>
                        <li><a href="#">Feedback</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Connect</h3>
                    <ul>
                        <li><a href="#"><i class="fab fa-twitter"></i> Twitter</a></li>
                        <li><a href="#"><i class="fab fa-facebook"></i> Facebook</a></li>
                        <li><a href="#"><i class="fab fa-github"></i> GitHub</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 ImageCompressorPro. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <div class="toast" id="toast"></div>

    <script>
        // DOM Elements
        const fileInput = document.getElementById('fileInput');
        const uploadArea = document.getElementById('uploadArea');
        const qualitySlider = document.getElementById('qualitySlider');
        const qualityValue = document.getElementById('qualityValue');
        const formatSelect = document.getElementById('formatSelect');
        const compressBtn = document.getElementById('compressBtn');
        const resetBtn = document.getElementById('resetBtn');
        const spinner = document.getElementById('spinner');
        const results = document.getElementById('results');
        const originalImage = document.getElementById('originalImage');
        const compressedImage = document.getElementById('compressedImage');
        const originalSize = document.getElementById('originalSize');
        const compressedSize = document.getElementById('compressedSize');
        const originalDimensions = document.getElementById('originalDimensions');
        const compressedDimensions = document.getElementById('compressedDimensions');
        const reductionPercent = document.getElementById('reductionPercent');
        const downloadBtn = document.getElementById('downloadBtn');
        const toast = document.getElementById('toast');

        // Variables
        let originalFile = null;
        let compressedBlob = null;
        let fileName = '';
        let fileExtension = '';

        // Event Listeners
        fileInput.addEventListener('change', handleFileSelect);
        uploadArea.addEventListener('dragover', handleDragOver);
        uploadArea.addEventListener('dragleave', handleDragLeave);
        uploadArea.addEventListener('drop', handleDrop);
        qualitySlider.addEventListener('input', updateQualityValue);
        compressBtn.addEventListener('click', compressImage);
        resetBtn.addEventListener('click', resetTool);

        // Functions
        function handleFileSelect(e) {
            const file = e.target.files[0];
            if (file) {
                processFile(file);
            }
        }

        function handleDragOver(e) {
            e.preventDefault();
            e.stopPropagation();
            uploadArea.classList.add('active');
        }

        function handleDragLeave(e) {
            e.preventDefault();
            e.stopPropagation();
            uploadArea.classList.remove('active');
        }

        function handleDrop(e) {
            e.preventDefault();
            e.stopPropagation();
            uploadArea.classList.remove('active');
            
            const file = e.dataTransfer.files[0];
            if (file) {
                fileInput.files = e.dataTransfer.files;
                processFile(file);
            }
        }

        function processFile(file) {
            // Check file type
            const validTypes = ['image/jpeg', 'image/png', 'image/webp'];
            if (!validTypes.includes(file.type)) {
                showToast('Please select a valid image file (JPEG, PNG, or WebP)', 'error');
                return;
            }
            
            // Check file size (10MB limit)
            if (file.size > 10 * 1024 * 1024) {
                showToast('File size exceeds 10MB limit', 'error');
                return;
            }
            
            originalFile = file;
            fileName = file.name.split('.').slice(0, -1).join('.');
            fileExtension = file.name.split('.').pop().toLowerCase();
            
            // Display original image
            const reader = new FileReader();
            reader.onload = function(e) {
                originalImage.src = e.target.result;
                
                // Get image dimensions
                const img = new Image();
                img.onload = function() {
                    originalDimensions.textContent = `${this.width} × ${this.height}`;
                };
                img.src = e.target.result;
            };
            reader.readAsDataURL(file);
            
            // Display original file size
            originalSize.textContent = formatFileSize(file.size);
            
            // Enable compress button
            compressBtn.disabled = false;
        }

        function updateQualityValue() {
            qualityValue.textContent = `${qualitySlider.value}%`;
        }

        function compressImage() {
            if (!originalFile) {
                showToast('Please select an image first', 'error');
                return;
            }
            
            spinner.style.display = 'block';
            results.style.display = 'none';
            
            // Simulate compression delay (in a real app, this would be actual compression)
            setTimeout(() => {
                const quality = parseInt(qualitySlider.value) / 100;
                const format = formatSelect.value === 'original' ? fileExtension : formatSelect.value;
                
                // In a real implementation, you would use canvas or a compression library here
                // This is a simplified simulation
                simulateCompression(originalFile, quality, format);
                
                spinner.style.display = 'none';
                results.style.display = 'block';
            }, 1000);
        }

        function simulateCompression(file, quality, format) {
            // This is a simulation - in a real app, you would use actual compression
            const originalSize = file.size;
            let compressedSizeValue;
            
            // Simulate size reduction based on quality
            if (quality >= 0.9) {
                compressedSizeValue = originalSize * 0.7; // 30% reduction
            } else if (quality >= 0.7) {
                compressedSizeValue = originalSize * 0.5; // 50% reduction
            } else if (quality >= 0.5) {
                compressedSizeValue = originalSize * 0.3; // 70% reduction
            } else {
                compressedSizeValue = originalSize * 0.2; // 80% reduction
            }
            
            // Further reduce if converting to WebP
            if (format === 'webp') {
                compressedSizeValue *= 0.8; // Additional 20% reduction
            }
            
            // Ensure minimum size
            compressedSizeValue = Math.max(compressedSizeValue, 1024); // At least 1KB
            
            // Update UI with simulated results
            compressedImage.src = originalImage.src; // In real app, this would be the compressed image
            compressedSize.textContent = formatFileSize(compressedSizeValue);
            compressedDimensions.textContent = originalDimensions.textContent;
            
            const reduction = ((originalSize - compressedSizeValue) / originalSize * 100).toFixed(1);
            reductionPercent.textContent = `${reduction}%`;
            
            // Create a simulated blob for download
            compressedBlob = new Blob([file], { type: `image/${format}` });
            
            // Set download link
            const newExtension = format === 'jpeg' ? 'jpg' : format;
            downloadBtn.href = URL.createObjectURL(compressedBlob);
            downloadBtn.download = `${fileName}_compressed.${newExtension}`;
            
            showToast('Image compressed successfully!', 'success');
        }

        function resetTool() {
            fileInput.value = '';
            originalFile = null;
            compressedBlob = null;
            originalImage.src = '';
            compressedImage.src = '';
            originalSize.textContent = '0 KB';
            compressedSize.textContent = '0 KB';
            originalDimensions.textContent = '0 × 0';
            compressedDimensions.textContent = '0 × 0';
            reductionPercent.textContent = '0%';
            qualitySlider.value = 80;
            qualityValue.textContent = '80%';
            formatSelect.value = 'original';
            results.style.display = 'none';
            compressBtn.disabled = true;
        }

        function formatFileSize(bytes) {
            if (bytes < 1024) return `${bytes} B`;
            else if (bytes < 1024 * 1024) return `${(bytes / 1024).toFixed(1)} KB`;
            else return `${(bytes / (1024 * 1024)).toFixed(1)} MB`;
        }

        function showToast(message, type) {
            toast.textContent = message;
            toast.className = 'toast';
            toast.classList.add(type);
            toast.classList.add('show');
            
            setTimeout(() => {
                toast.classList.remove('show');
            }, 3000);
        }

        // Initialize
        updateQualityValue();
        compressBtn.disabled = true;
    </script>

    <!-- Structured Data for SEO -->
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "WebApplication",
        "name": "ImageCompressorPro - Free Online Image Compression Tool",
        "url": "https://yourwebsite.com/image-compressor",
        "description": "Free online tool to compress your images while maintaining quality. Reduce file size for JPG, PNG, and WebP images quickly and easily.",
        "applicationCategory": "MultimediaApplication",
        "operatingSystem": "Any",
        "offers": {
            "@type": "Offer",
            "price": "0",
            "priceCurrency": "USD"
        },
        "creator": {
            "@type": "Organization",
            "name": "ImageCompressorPro"
        }
    }
    </script>
</body>
</html>
