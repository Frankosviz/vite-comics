<template>
    <div class="fd-followUs-style">
        <div class="container d-flex justify-content-between">
            <div class="d-flex pt-5 ">
                <div>
                    <ul>
                        <h2>Dc Comics</h2>
                        <li v-for="(item, index) in arrayDcComics" :key="index">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                    <ul>
                        <h2>Shop</h2>
                        <li v-for="(item, index) in arrayShop" :key="index">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <h2>DC</h2>
                        <li v-for="(item, index) in arrayDc" :key="index">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <h2>Sites</h2>
                        <li v-for="(item, index) in arraySites" :key="index">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>

            </div>
            <div class="position-relative cropped">
                <img src="../../public/img/dc-logo-bg.png" alt="DC-Background-image">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FollowUsComponent',
    data() {
        return {
            arrayDcComics: [
                {
                    name: 'Characters',
                    url: '#'
                },
                {
                    name: 'Comics',
                    url: '#'
                },
                {
                    name: 'Movies',
                    url: '#'
                },
                {
                    name: 'TV',
                    url: '#'
                },
                {
                    name: 'Games',
                    url: '#'
                },
                {
                    name: 'Videos',
                    url: '#'
                },
            ],

            arrayDc: [
                {
                    name: 'Terms of Use',
                    url: '#'
                },
                {
                    name: 'Privacy policy (New)',
                    url: '#'
                },
                {
                    name: 'Ad Choices',
                    url: '#'
                },
                {
                    name: 'Advertising',
                    url: '#'
                },
                {
                    name: 'Jobs',
                    url: '#'
                },
                {
                    name: 'Subscriptions',
                    url: '#'
                },
                {
                    name: 'Talent Workshops',
                    url: '#'
                },
                {
                    name: 'CPSC Certificates',
                    url: '#'
                },
                {
                    name: 'Ratings',
                    url: '#'
                },
                {
                    name: 'Shop Help',
                    url: '#'
                },
                {
                    name: 'Contact Us',
                    url: '#'
                }
            ],

            arraySites: [
                {
                    name: 'DC',
                    url: '#'
                },
                {
                    name: 'MAD Magazine',
                    url: '#'
                },
                {
                    name: 'DC Kids',
                    url: '#'
                },
                {
                    name: 'DC Universe',
                    url: '#'
                },
                {
                    name: 'DC Power Visa',
                    url: '#'
                }
            ],

            arrayShop: [
                {
                    name: 'Shop DC',
                    url: '#'
                },
                {
                    name: 'Shop DC Collectibles',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
.fd-followUs-style {
    height: 450px;
    background-image: url('../../public/img/footer-bg.jpg');
    background-size: cover;
}

h2 {
    color: white;
    font-size: 20px;
    text-transform: uppercase;
}

img {
    position: absolute;
    right: 0;
    top: -80px;
}

.cropped {
    width: 600px;
    height: 450px;
    overflow: hidden;
}

ul {
    list-style-type: none;
    line-height: 30px;
    color: white;
}

a {
    text-decoration: none;
    color: $textcolor;
    font-weight: normal;
    font-size: 13px;
}
</style>