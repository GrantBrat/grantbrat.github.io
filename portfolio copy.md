---
layout: page
title: Portfolio
toc: yes
---

<style>
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
        gap: 20px;
        justify-items: center;
    }
    .grid-item {
        position: relative; /* Ensure relative positioning for overlay */
    }
    .grid-item img {
        max-width: 100%;
        height: auto;
        border-radius: var(--border-radius); /* Use the border-radius defined in your CSS */
        box-shadow: inset 0 0 0 1px rgba(255,255,255,.15); /* Example box shadow */
        cursor: pointer; /* Add cursor pointer to indicate clickable */
    }
    .grid-item .overlay {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.5); /* Semi-transparent overlay */
        display: flex;
        justify-content: center;
        align-items: center;
        opacity: 0; /* Initially hidden */
        transition: opacity 0.3s ease; /* Smooth transition for overlay */
    }
    .grid-item:hover .overlay {
        opacity: 1; /* Show overlay on hover */
    }
    .grid-item .overlay a {
        display: block;
        color: white;
        text-decoration: none;
        font-size: 18px;
        font-weight: bold;
    }
</style>

<div class="grid-container">
    <div class="grid-item">
        <img src="/assets/senior3.jpg" alt="Senior Photo 1">
        <div class="overlay">
            <a href="/assets/senior3.jpg" target="_blank">View in New Tab</a>
        </div>
    </div>
    <div class="grid-item">
        <img src="/assets/senior4.jpg" alt="Senior Photo 2">
        <div class="overlay">
            <a href="/assets/senior4.jpg" target="_blank">View in New Tab</a>
        </div>
    </div>
    <!-- Repeat for other images -->
</div>

<!-- Repeat the same structure for other sections (Weddings, Portraits, Dogs, Misc) -->
