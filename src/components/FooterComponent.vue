
import { RouterLink } from 'vue-router';
<template>
    <footer class="amazing-footer">
        <div class="footer-contact">
            <div class="footer-section">
                <h4>About Me</h4>
                <p style="max-width: 70%;">
                    Passionate Web Developer and Programmer with over 5 years of experience in creating dynamic and responsive websites.
                    Specialize in "React, Vue.js and Node.js" for Web Development, and proficient in C++, Python and Javascript.
                </p>
            </div>
            <div class="footer-quicklinks">
                <h4>Quick Links</h4>
                <ul>
                    <li><RouterLink class="footer-link" to="/">Home</RouterLink> </li>
                    <li><RouterLink class="footer-link" to="/about">About</RouterLink> </li>
                    <li><RouterLink class="footer-link" to="/contact">Contact Me</RouterLink> </li>
                </ul>
            </div>
            <div class="footer-details">
                <h4>Contact Info</h4>
                <p><i class="fas fa-map-marker-alt"></i> 22 Mia Mia Way, Torquay</p>
                <p><i class="fas fa-phone"></i> +61 412 925 415</p>
                <p><i class="fas fa-envelope"></i> jai.knight2001@gmail.com</p>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; Jai. All rights reserved.</p>
        </div>
    </footer>
</template>

<script>

</script>