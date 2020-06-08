<template>
    <footer class="pb-5 bg-primary-3 text-light">
        <div class="container">
            <div class="row justify-content-center text-center">
                <div class="col-xl-10">
                    <small class="text-muted footer__copyright ">
                        ©{{getDate}} Building Hub Podcast. All Rights Reserved. 
                        <a class="footer__link">
                            Made with <span>❤</span> by 
                            <a href="" target="_blank" rel="noopener noreferrer">Samuel Sanni</a>
                        </a>
                    </small>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    computed: {
        getDate() {
            let date = new Date();
            return date.getFullYear();
        }
    },
}
</script>

<style scoped>
.footer__copyright span {
    color: rgb(220, 20, 60);
}

.footer__link {
    margin-left: 2rem;
    position: relative;
}

.footer__link::before {
    content: "";
    display: inline-block;
    width: 3px;
    height: 3px;
    background-color: rgb(255, 255, 255);
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    left: -1.2rem;
    border-radius: 100%;
}

@media (max-width: 992px) {
    .footer__link::before {
        top: 20%;
    }
}
</style>