    <script setup>

    const  footerLinks = [
        { linkItem: 'home', linkAddress: 'youtube.com' },
        { linkItem: 'contact', linkAddress: '' }, 
        { linkItem: 'city', linkAddress: '' }, 
        { linkItem: 'social media', linkAddress: '' },
    ];


    const props = defineProps({
        title: {
            type: String
        },
        pageLinks: {
            type: String
        }
    });
    
    </script>
    
    <template>
    
    <section class="footer" id="contact">
        
        <div class="footer-text">
            <h1>{{title}}</h1>
            <li v-for="links in footerLinks"><a href="">{{links.linkItem}}</a></li>
        </div>
    </section>
    
    
    
    </template>
    
    <style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');
    
    .footer {
        background-image: linear-gradient(to right top, #365c3a, #01584e, #00515f, #0b4764, #363a5c);
        margin: auto;
        font-family: 'Work Sans', sans-serif;
        position: relative;
    }
    
    h1 {
        font-size: 2rem;
        color: #FCFAFB;
        margin-bottom: 40px;
    }
    
    .footer-text {
        max-width: 1000px;
        margin: auto;
        font-size: 1.1rem;
        padding: 100px 0;
        color: #FCFAFB;
    }

    li {
        list-style: none;
    }
    
    a {
        text-decoration: none;
        color: #fff;
        display: inline-block;
        padding: 5px 10px;
        margin-bottom: 20px;
    }

    a:hover {
        border: 1px solid #fff;
        padding: 4px 9px;
    }

    @media screen and (max-width: 480px) {
        .footer {
            padding: 15px;
        }

        .footer-text {
            padding: 20px 15px;
        }

        a {
            padding: 0;
        }

    }

    </style>