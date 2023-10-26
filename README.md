
# Weekly Assignment Week2

**Deliverables**

Basic Website with HTML, CSS, simple Javascript and responsive website.

**Task**

1. Implement basic CSS to style your website. 
2. Add simple JavaScript functionality to enhance user interactions.
3. Create a functional form on your website that includes input types (text, textarea), a submit button, and at least one of the following: radio buttons, checkboxes, or a select dropdown.
4. Style your form to align with your website's design.
5. Deploy website
6. Create a responsive website, minimal 2 category (Dekstop and mobile)


---
</br>

## My Wesbsite 

### About Content

Discusses material final processing services in various ways, especially special treatment of materials whose main ingredient is iron. The aim that the resulting material will be strong and corrosion resistant.

**Website Design Content**

1. Heading contains the logo, desktop and mobile menu navigation, and shop front display
    ```html
        <header id="header" class="first-header">

                <nav class="navbar">
                    <span class="main-logo">
                        <img src="/assets/Metal-Ball-logo.png"
                            alt="surface plating logo"            
                            style="width:40px; height:40px;"/>       
                        <b><em>SURFACE PLATING SERVICE</em></b>
                        <span class="copyright">&copy</span>
                    </span>
                
                    <ul class="menu-bar">
                        <li><a href="#header">Home</a></li>
                        <li><a href="#layanan">Our Services</a></li>
                        <li><a href="#product-picture">Available Project</a></li>
                        <li><a href="#kontak">Contact</a></li>
                    </ul>
            
                    <div class="mobile">
                        <img
                        src="https://user-images.githubusercontent.com/2970318/209647125-dc41103d-c545-4e2e-b89b-099fbfcde702.svg"
                        alt="Hamburger Icon"
                        />

                        <ul id="menu">
                            <a href="#header"><li>Home</li></a>
                            <a href="#layanan"><li>Our Services</li></a>
                            <a href="#product-picture"><li>Available Project</li></a>
                            <a href="#kontak"><li>Contact</li></a>
                            <a href="https://github.com/imanmaris99" target="_blank"><li>Show me more</li></a>
                        </ul>
                    </div>  
                </nav>

                <div class="mading-1">    
                    <h1>SURFACE PLATING SOLUTIONS</h1>     
                    <p>Meningkatkan Kualitas dan Tahan Lama Produk Anda</p>
                </div>

            </header>
    ```
2. Main Display is divided into 4 contents, including 1 article and 5 sections
    ```html
        <main>
            <article>
                <h2>ABOUT US</h2>
                <p class="benefits">....</p>

            </article>

            <section id="layanan">
                <h2>OUR SERVICES</h2>
                <div class="layanan-item1">....</div>
                <div class="layanan-item2">....</div>
    
            </section>

            <section id="product-picture">
                <h2  style="font-family: roboto; padding-top: 1%; text-align: center;">OUR PROJECT</h2>
                <h3>Various Types of <mark>ELECTROPLATING</mark> are available here</h3>
                <div class="proyek-item">
                    <ul class="menu-bar">
                        <li><a href=".layanan-item3">Type I: Chromium Plating</a></li>
                        <li><a href=".layanan-item4">Type II: Zinc Plating</a></li>
                        <li><a href=".layanan-item5">Type III: Nickel Plating</a></li>
                    </ul>
                </div>    

                <div class="grid-container">....</div>

                <!------------------------------------------FITURE FOR MOBILE ------------------------------------------>

                <div class="w3-content w3-display-container">....</div>
                <!--------------------------------------------------MOBILE END----------------------------------------------->

            </section>


            <section id="product-picture-2">
                <h3>Various Types of <mark>ANODIZING</mark> are available here</h3>
                <div class="proyek-item-2">
                    <ul class="menu-bar-2">
                        <li><a href=".layanan-item3">Type I: Chromic Acid Anodizing</a></li>
                        <li><a href=".layanan-item4">Type II: Sulfuric Acid Anodizing</a></li>
                        <li><a href=".layanan-item5">Type III: Hard Anodizing</a></li>
                    </ul>
                </div>

                <div class="grid-container-2">....</div>

                <!------------------------------------------FITURE FOR MOBILE ------------------------------------------>

                <div class="w3-content w3-display-container"> .... </div>
                <!--------------------------------------------------MOBILE END----------------------------------------------->

            </section>

            <section id="proses-produksi">
                <h2>PRODUCTION PROCESS</h2>
                <div class="produksi">

                </div>   
            </section>
        
            <section id="kontak">
                <h2>CONTACT US</h2>
                
                <form>
                    <fieldset>
                        <legend>Personal Data:</legend>
                    </fieldset>
                </form>

                <address>
                    Shop Adress: Jl. Mangkudipuro No. 123, City of Pati, Code Post 59185
                    Telp.: (123) 456-7890
                    Email: info@surfaceplating.com
                </address>

            </section>

        </main>
    ```
3. Footer.
    ```html
        <footer class="last-footer">
            <p>....</p>
        </footer>
        
    ```
    <br>

**Website Design Responsive**

Responsive mode available on desktop and mobile
```css
    @media only screen and (max-width: 700px) {
        /* For mobiles: */
        
        nav {
            position: fixed;
            width: 100%;
            justify-content: space-between;
            height: 8%;
            background-color: #e5d183ec;
            z-index: 12;
        }

        nav .mobile{
            padding-right: 5%;
            display: flex;
            position:static;
        }

        nav > ul {
            display: none;
            }
        
        .mading-1>h1{
            padding-top: 25%;
            justify-content: center;
            text-align: center;
        }

        /*------------------------------------------------*/

        /* Konten Dropdown (Hidden secara Default) */

        .mobile ul {
            display: none;
            position: absolute;
            background-color: #e5d183ec;
            width: 100%;
            margin: -10px -440px;
            height: 500%;
            padding: 70px;
            padding-top: 80px;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            z-index: -10;
        }

        #product-picture {
            padding-bottom: 15%;
            background-color: #F5F7F8;
        }

        #product-picture .grid-container{
            display: none;
        }

        #product-picture-2 .grid-container-2{
            display: none;

        }

        #product-picture-2 {
            margin-top: 0%;
            padding-bottom: 15%;
            background-color: #F5F7F8;
        }

        #product-picture .w3-content{
            display:flex;
            position:static;
            align-items:stretch;
            justify-content: center;
        }

        #product-picture .w3-content img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        #product-picture-2 .w3-content{
            display:flex;
            position:static;
            align-items:stretch;
            justify-content: center;
        }

        #product-picture-2 .w3-content img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        #proses-produksi{
            margin-top: 5%;
            background-color: #F5F7F8;
            padding-top: 20px;
            padding-bottom: 5%;
        } 

        #proses-produksi h2{
            text-align: center;
            padding-bottom: 10%;
        }
        
        #proses-produksi iframe{
            text-align: center;
            padding-top: 5%;
            padding-bottom: 2%;
        }

        #kontak h2{
            margin-top: 5%;
            background-color: #F5F7F8;
            padding-top: 10px;
            padding-bottom: 10%;
        }

        form fieldset{
            padding: 20px 10px 10px 10px;

        }

        form fieldset legend{
            padding: 10px;
            text-align: center;

        }
    }

```
<br>

**Equipment Used Design Content**

|      Tools     |
|----------------|
|![Html](https://cdn-icons-png.flaticon.com/128/5968/5968267.png) ![CSS](https://cdn-icons-png.flaticon.com/128/5968/5968242.png) ![Javascript](https://cdn-icons-png.flaticon.com/128/5968/5968292.png) |

<br>

**Equipment Used to Deploy Content**

|       Tool     | Tool Website | My Link Website|
|----------------|--------------|----------------|
|<img width="30%" src="https://logowik.com/content/uploads/images/vercel1868.jpg">|[Vercel](https://vercel.com/)|[Assignment-week2](https://module-1-imanmaris.vercel.app/)|
|<img width="30%" src="https://pbs.twimg.com/profile_images/1633183038140981248/Mz4bv8Ja_400x400.png">|[Netlify](https:///)|[Assignment-week2](https://delightful-pixie-c253af.netlify.app/)|




<br>
<br>

---



<p align="center">last created on October 27, 2023</p>
<p align="center"><i>copyright &copy; 2023</i></p>


