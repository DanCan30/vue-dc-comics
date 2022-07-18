<template>
  <section>
    <div>
        <div class="social-left">
            <a href="#">sign-up now!</a>
        </div>
        <div class="social-right">
            <a class="follow-us" href="#">follow us</a>
            <ul>
                <li v-for="(social, index) in socialLinks" :key="index">
                    <a href="social.url">
                        <img :src="require(`../assets/img/footer${social.src}`)" alt="social.text">
                        </a>
                </li>
            </ul>
        
        </div>
    </div>
  </section>
</template>

<script>
export default {
    data: function() {
        return {
            socialLinks: [
                {
                    src: "-facebook.png",
                    url: "#",
                    text: "facebook",
                },
                {
                    src: "-twitter.png",
                    url: "#",
                    text: "twitter",
                },
                {
                    src: "-youtube.png",
                    url: "#",
                    text: "youtube",
                },
                {
                    src: "-pinterest.png",
                    url: "#",
                    text: "pinterest",
                },
                {
                    src: "-periscope.png",
                    url: "#",
                    text: "periscope",
                },
                
            ]
        }
    }
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


                ul {
                    list-style: none;

                    li {
                        display: inline-block;
                    }
                }

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