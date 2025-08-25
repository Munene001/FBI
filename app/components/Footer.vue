<script setup lang="ts">
import { NuxtLink } from '#components';
</script>

<template>
    <div class="bg-[#8A2B1A]  flex flex-col font-[uno] text-white px-6 gap-10 py-8 md:py-14 md:items-start md:flex-row md:px-12" id="footer">
        <!-- Logo and Mission -->
        <div class="flex flex-col gap-6 md:flex-1">
            <div class="flex items-center gap-4">
                <img src="/l.jpeg" alt="FBI logo" class="h-14 w-14">
                <div class="text-2xl font-bold tracking-wide">FBI kenya</div>
            </div>
            <div class="text-base leading-relaxed font-light border-l-4 border-white pl-4 py-2">
                We are the people's movement fighting for justice, equality and systemic change. 
                Join us in building power through collective action and grassroots organizing.
            </div>
            <div class="flex gap-4">
                <NuxtLink to="/contact" class="bg-white text-[#8A2B1A] px-6 py-2 rounded font-medium hover:bg-gray-100 transition">
                    Join Now
                </NuxtLink>
            </div>
        </div>

        <!-- Navigation Columns -->
        <div class="grid grid-cols-2 gap-8 md:flex-1">
            <div class="flex flex-col gap-4">
                <h3 class="text-xl font-bold uppercase tracking-wider">Our Work</h3>
                <div class="flex flex-col gap-3 text-base font-light">
                    <NuxtLink to="/about" class="hover:text-gray-300 transition">About</NuxtLink>
                    <NuxtLink to="/about" class="hover:text-gray-300 transition">Direct Actions</NuxtLink>
                    <NuxtLink to="/about" class="hover:text-gray-300 transition">Political Education</NuxtLink>
                    <NuxtLink to="/dashboard" class="hover:text-gray-300 transition">Dashboard</NuxtLink>
                </div>
            </div>

            <div class="flex flex-col gap-4">
                <h3 class="text-xl font-bold uppercase tracking-wider">Resources</h3>
                <div class="flex flex-col gap-3 text-base font-light">
                   
                    <NuxtLink to="/manifesto" class="hover:text-gray-300 transition">Our Manifesto</NuxtLink>
                    <NuxtLink to="/contact" class="hover:text-gray-300 transition">FAQS</NuxtLink>
                    <NuxtLink to="/contact" class="hover:text-gray-300 transition">Contact Us</NuxtLink>
                </div>
            </div>
        </div>

        <!-- Contact and Social -->
        <div class="flex flex-col gap-6 md:flex-1">
            <div class="flex flex-col gap-4">
                <h3 class="text-xl font-bold uppercase tracking-wider">Connect</h3>
                <div class="flex flex-col gap-2 text-base font-light">
                    <div>draintheswamp@fbikenya.org</div>
                    <div>+254714191919</div>
                    <div>Nairobi, Kenya</div>
                </div>
            </div>

            <div class="flex flex-col gap-4">
                <h3 class="text-xl font-bold uppercase tracking-wider">Follow</h3>
                <div class="flex gap-4">
                    <NuxtLink to="https://twitter.com" class="hover:opacity-80 transition">
                        <span class="sr-only">Twitter</span>
                        <span class="text-2xl">𝕏</span>
                    </NuxtLink>
                    <NuxtLink to="https://instagram.com" class="hover:opacity-80 transition">
                        <span class="sr-only">Instagram</span>
                        <span class="text-2xl">📸</span>
                    </NuxtLink>
                    <NuxtLink to="https://t.me" class="hover:opacity-80 transition">
                        <span class="sr-only">Telegram</span>
                        <span class="text-2xl">✉️</span>
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>

    <div class="bg-[#5E1C12] text-white font-[uno] text-center py-5 border-t border-[#A03A2B]">
        <div class="container mx-auto px-6">
            © 2025 FBI Kenya | Power to the People | 
            <NuxtLink to="" class="hover:underline ml-2">Privacy Policy</NuxtLink>
        </div>
    </div>
</template>