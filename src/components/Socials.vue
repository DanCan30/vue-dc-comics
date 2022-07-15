<template>
  <section>
    <div>
        <div class="social-left">
            <a href="#">sign-up now!</a>
        </div>
        <div class="social-right">
            <a href="#">follow us</a>
            <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
            <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
            <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
            <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
            <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
        </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

@import "../stiles/mixins.scss";
@import "../stiles/variables.scss";

    section {
        background-color: #303030;

        &>div {
            @include generalContainer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 3rem 0;

            a {
                text-decoration: none;
            }

            .social-left {
                width: 50%;

                a {
                    color: white;
                    display: inline-block;
                    padding: .75rem;
                    border: 2px solid $brandColor;
                    text-transform: uppercase;
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
                    font-size: 1.2rem;
                    padding: 0 1rem;
                }
            }
        }
    }
</style>