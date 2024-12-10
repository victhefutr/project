<div class="news-ticker">
    <div class="ticker-content">
        <span class="ticker-icon">🌟</span>
        Special Offer: <span class="discount-highlight">40% OFF</span> for New Residents - Comfort and Care Await! Limited Time Offer Only at Our Care Home 🏡
    </div>
</div>


<style>
    .news-ticker {
            background: linear-gradient(to right, #2563eb, #4338ca);
            color: white;
            padding: 15px 0;
            overflow: hidden;
            position: relative;
            width: 100%;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

    .ticker-content {
        display: inline-block;
        white-space: nowrap;
        padding-left: 100%;
        animation: ticker 20s linear infinite;
    }

    .ticker-content:hover {
        animation-play-state: paused;
    }

    @keyframes ticker {
        0% {
            transform: translate(0, 0);
        }
        100% {
            transform: translate(-100%, 0);
        }
    }

    .ticker-icon {
        display: inline-block;
        margin-right: 10px;
        vertical-align: middle;
        animation: pulse 2s infinite;
    }

    @keyframes pulse {
        0%, 100% {
            transform: scale(1);
        }
        50% {
            transform: scale(1.1);
        }
    }

    .discount-highlight {
        font-weight: bold;
        color: #ffd700;
        margin: 0 5px;
    }
</style>