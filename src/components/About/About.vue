    <script setup>

    </script>
    
    <template>
    
    <section class="about">
        <div class="about-text">
            <h2>About Us</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Atque sit porro aspernatur voluptatem quia. Nemo at voluptas dolorem consectetur aperiam consequuntur cum amet quia deleniti ipsa mollitia, quaerat obcaecati dolor architecto repudiandae pariatur id excepturi magni quos eius tempore reprehenderit corporis! A labore tenetur necessitatibus laboriosam sed error praesentium dolores.</p>
        </div>
        
    </section>


    
    </template>
    
    <style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');
    
    .about {
        max-width: 1000px;
        margin: auto;
        font-family: 'Work Sans', sans-serif;
    }

    h2 {
        font-size: 1.2rem;
        color: #5C3636;
        margin-bottom: 20px;
    }

    .about-text {
        width: 50%;
        font-size: 1.1rem;
        line-height: 1.6;
        padding: 100px 0;
        color: #363A5C;
    }
    
    @media screen and (max-width: 480px) {
        .about {
            width: 80%;
            padding: 15px;
        }

        .about-text {
        width: 100%;
        margin: 20px 0;
        padding: 0;
        color: #363A5C;
        }
    }
    </style>