        // List of top 70 most used emojis
        const emojis = [
            "😀", "😂", "😍", "🥳", "🤔", "🙏", "🤣", "😊", "❤️", "😢",
            "😎", "🤯", "😱", "🤗", "😴", "🙈", "🙉", "🙊", "💪", "👌",
            "👏", "🙌", "🤲", "🤝", "💁", "🙆", "🙅", "🙇", "💃", "🕺",
            "👀", "👋", "✌️", "👍", "👎", "👊", "💋", "💘", "💝", "💖",
            "💗", "💓", "💞", "💕", "💟", "💌", "💍", "💎", "💐", "🔥",
            "💰", "👀", "📱", "💻", "🖥️", "📞", "📧", "🕶️", "📸", "💣",
            "🔒", "🔑", "🎉", "🏆", "📚", "🍎", "🍕", "🍔", "🌮", "🍣"
        ];

        // Function to get 5 random unique emojis
        function getRandomEmojis() {
            const selectedEmojis = [];
            while (selectedEmojis.length < 5) {
                const randomIndex = Math.floor(Math.random() * emojis.length);
                const emoji = emojis[randomIndex];
                if (!selectedEmojis.includes(emoji)) {
                    selectedEmojis.push(emoji);
                }
            }
            return selectedEmojis;
        }

        // Update emojis and apply bounce effect
        function updateEmojis() {
            const newEmojis = getRandomEmojis();
            const emojiElements = document.querySelectorAll('.emoji');
            emojiElements.forEach((element, index) => {
                element.classList.add('bounce');
                setTimeout(() => {
                    element.textContent = newEmojis[index];
                    element.classList.remove('bounce');
                }, 500); // Delay to match animation duration
            });
        }

        // Add click event to change emojis
        document.getElementById('logo-link').addEventListener('click', (event) => {
            event.preventDefault(); // Prevent default link behavior
            updateEmojis();
        });
   
