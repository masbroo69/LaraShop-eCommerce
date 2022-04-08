<p dir="auto" align="center"><a href="http://www.ruangsebelah.com/" rel="nofollow"><img src="https://i.postimg.cc/NLvHNwcR/logo-top-1.png" style="max-width: 30%;" width="30%"></a></p>

<p dir="auto" align="center"><a href="https://i.postimg.cc/ydfjrxQc/Fire-Shot-Capture-036-Lara-Shop-Home-localhost.png/" rel="nofollow"><img src="https://i.postimg.cc/ydfjrxQc/Fire-Shot-Capture-036-Lara-Shop-Home-localhost.png" style="max-width: 100%;"></a></p>

<div data-target="readme-toc.content" class="Box-body px-5 pb-5">
            <article class="markdown-body entry-content container-lg" itemprop="text">
<h1 dir="auto"><a id="user-content-laravel-ecommerce-example" class="anchor" aria-hidden="true" href="#laravel-ecommerce-example"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>
# LaraShop Ecommerce Example</h1>
<p> Laravel 9.6 Livewire eCommerce with RajaOngkir Shipment & Midtrans Gateway Payments</p>
<p dir="auto">Website Demo: <a href="https://youtu.be/1DehaNr3yUQ" rel="nofollow">https://www.ruangsebelah.com/</a>. The demo has limited permissions. Install locally for full access.</p>
<h2 dir="auto"><a id="user-content-installation" class="anchor" aria-hidden="true" href="#installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Installation</h2>
<ol dir="auto">
<li>Clone the repo and <code>cd</code> into it</li>
<li><code>composer install</code></li>
<li>Rename or copy <code>.env.example</code> file to <code>.env</code></li>
<li><code>php artisan key:generate</code></li>
<li>Set your database credentials in your <code>.env</code> file</li>
<li>Set your Midtrans credentials in your <code>.env</code> file. Specifically <code>MIDTRANS_SERVER_KEY</code> and <code>MIDTRANS_CLIENT_KEY</code></li>
<li>Set your RajaOngkir credentials in your <code>.env</code> file. Specifically <code>RAJAONGKIR_API_KEY</code> and <code>RAJAONGKIR_PACKAGE</code></code> and <code>RAJAONGKIR_ORIGIN</code></li>
<li>Set your Stripe credentials in your <code>.env</code> file. Specifically <code>STRIPE_KEY</code> and <code>STRIPE_SECRET</code></li>            
<li>Set your PayPal credentials in your <code>.env</code> file. Specifically <code>STRIPE_KEY</code> and <code>STRIPE_SECRET</code></li> This will migrate the database and run any seeders necessary. See <a href="https://www.youtube.com/watch?v=xfSks-NdHPw&list=PLz_YkiqIHesvPtvLl2Wz5FtuW44dBt199" rel="nofollow">this episode</a>.</li>
<li><code>npm install</code></li>
<li><code>npm run dev</code></li>
<li><code>php artisan migrate:fresh --seed</code></li>
<li><code>php artisan serve</code> or use Laravel Valet or Laravel Homestead</li>
<li>Visit <code>localhost:8000</code> in your browser</li>
<li>Visit <code>/login</code> if you want to access the admin backend. Admin User/Password: <code>admin@admin.com/password</code>. Admin Web User/Password: <code>adminweb@adminweb.com/password</code></li>
</ol>
<h2 dir="auto"><a id="user-content-shopping-cart-package" class="anchor" aria-hidden="true" href="#shopping-cart-package"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Shopping Cart Package</h2>
<p dir="auto">I originally used the <a href="https://github.com/Crinsane/LaravelShoppingcart">Crinsane/LaravelShoppingcart</a> package but it is slow to update to the latest versions of Laravel. I now use <a href="https://github.com/hardevine/LaravelShoppingcart">hardevine/LaravelShoppingcart</a> which is a forked version that updates quicker.</p>
<h2 dir="auto"><a id="user-content-windows-users---money_format-issue" class="anchor" aria-hidden="true" href="#windows-users---money_format-issue"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Windows Users - money_format() issue</h2>
<p dir="auto">The <code>money_format</code> function does not work in Windows. Take a look at <a href="https://stackoverflow.com/questions/6369887/alternative-to-money-format-function-in-php-on-windows-platform/18990145" rel="nofollow">this thread</a>. As an alternative, just use the <code>number_format</code> function instead.</p>
<ol dir="auto">
<li>In <code>app/helpers.php</code> replace <code>money_format</code> line with <code>return '$'.number_format($price / 100, 2);</code></li>
<li>In <code>app/Product.php</code> replace <code>money_format</code> line with <code>return '$'.number_format($this-&gt;price / 100, 2);</code></li>
<li>In <code>config/cart.php</code> set the <code>thousand_seperator</code> to an empty string or you might get a 'non well formed numeric value encountered' error. It conflicts with <code>number_format</code>.</li>
</ol>
<h2 dir="auto"><a id="user-content-starting-from-a-particular-point" class="anchor" aria-hidden="true" href="#starting-from-a-particular-point"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Starting from a particular point</h2>
<p dir="auto">If you would like to follow along from a particular point, follow these instructions. I'm going to be starting from my starting point in the first video of the series. You can choose any point by replacing the hash with <a href="https://github.com/drehimself/laravel-ecommerce-example/commits/master">any particular commit</a>.</p>
<ol dir="auto">
<li>Clone the repo and <code>cd</code> into it</li>
<li><code>git checkout f4f651a8a35ebb2ff38ba15771fd65c93051f942</code></li>
<li>Follow the rest of the steps above. Instead of <code>php artisan ecommerce:install</code>, migrate and seed the normal way with <code>php artisan migrate --seed</code></li>
</ol>
</article>
          </div>
