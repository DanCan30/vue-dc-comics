<template>
  <section>
    <div>
        <div class="social-left">
            <a href="#">sign-up now!</a>
        </div>
        <div class="social-right">
            <a href="#">follow us</a>
            <a href=""><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
            <a href=""><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
            <a href=""><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
            <a href=""><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
            <a href=""><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
        </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

@import "../assets/stiles/mixins.scss";
@import "../assets/stiles/variables.scss";

    section {
        background-color: #303030;

        &>div {
            @include generalContainer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 2rem 0;

            a {
                text-decoration: none;
            }

            .social-left {
                width: 50%;

                a {
                    color: $brandSecondaryColor;
                    display: inline-block;
                    padding: .75rem 1rem;
                    border: 2px solid $brandColor;
                    text-transform: uppercase;
                    font-size: 1.3rem;
                }

            }

            .social-right {
                width: 50%;
                display: flex;
                justify-content: flex-end;
                align-items: center;

                a {
                    color: $brandColor;
                    text-transform: uppercase;
                    font-size: 1.3rem;
                    padding: 0 1rem;
                }
            }
        }
    }
</style>