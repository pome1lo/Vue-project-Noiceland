<template>
    <footer class="footer">
        <div class="top_section">
            <div class="footer_logo">
                <a href="#">
                    <img src="@/assets/LogoFooter.svg" alt="" />
                </a>
            </div>
            <p>© 2018 Noiceland™, all rights reserved</p>
        </div>
        <div class="buttom_section">
            <div class="footnote footnote-text">Categories</div>
            <div class="footnote-text">Subscribe to newsletter</div>
            <ul>
                <li><a href="#">Animation</a></li>
                <li><a href="#">Interactive Design</a></li>
            </ul>
            <ul>
                <li><a href="#">Architecture</a></li>
                <li><a href="#">Miscellaneous</a></li>
            </ul>
            <ul>
                <li><a href="#">Graphic Design</a></li>
                <li><a href="#">Photography</a></li>
            </ul>
            <ul>
                <li><a href="#">Illustration</a></li>
                <li><a href="#">Product Design</a></li>
            </ul>
            <form role="search">
                <input id="search" type="search" placeholder="Email address" autofocus required />
                <button type="submit">Send</button>    
            </form>
            <div class="footnote-text">Information</div>
            <div class="footnote-text">follow us</div>
            <div class="footnote-text last-child">Template</div>
            <ul>
                <li><a href="#">about</a></li>
                <li><a href="#">contact</a></li>
                <li><a href="#">terms</a></li>
            </ul>
            <ul>
                <li><a href="#">instagram</a></li>
                <li><a href="#">facebook</a></li>
                <li><a href="#">twitter</a></li>
            </ul>
            <ul>
                <li><a href="#">Image License Info</a></li>
                <li><a href="#">Powered by Webflow</a></li>
            </ul>
        </div>
    </footer>
</template>

<style scoped lang="scss">
    footer {
        width: 100%;
        background-color: #141414;
        .top_section {
            padding: 70px 10px 35px 10px;
            display: flex;
            justify-content:left;
            border-bottom: 2px solid #4D4D4D;
            p {
                margin: 10px;
                font-family: 'Libre Franklin';
                font-style: normal;
                font-weight: 400;
                font-size: 10px;
                line-height: 12px;
                letter-spacing: 1px;
                text-transform: uppercase;
                color: #666666;
            }
        }
        .top_section,
        .buttom_section {
            width: 80%;
            margin: 0 10%;
        }
        .buttom_section {
            display: grid;
            padding: 0 0 80px 0;
            grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
            ul li {
                text-align: left;
                padding: 5px;
                :hover {
                        transition: .5s;
                        color: darkred;
                    }
                a { 
                    color: white; 
                    font-family: 'Libre Franklin';
                }
            }
            form {
                margin: auto;
                display: flex;
                justify-content: left;
                align-items: center;
                width: 100%;
                color: white;
                input {
                    padding: 10px;
                }
                button {
                    padding: 10px;
                    background-color: #000000;
                    color: white;
                }
            }
            .footnote-text {
                color: #666666;
                text-transform: uppercase;
                font-family: 'Libre Franklin';
                font-style: normal;
                font-weight: 400;
                line-height: 12px;
                text-align: left;
                padding: 25px 0;
            }
            .last-child {
               grid-column-start: 3;
               grid-column-end: 6;
           }
            .footnote {
                grid-column-start: 1;
                grid-column-end: 5;
            }
            
        }
    }
</style>