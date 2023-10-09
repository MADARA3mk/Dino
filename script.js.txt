document.addEventListener('keydown', jump);

function jump(event) {
    if (event.keyCode === 32) { // Spacebar
        const dino = document.querySelector('.dino');
        dino.style.animation = 'jump 1s';
        setTimeout(() => {
            dino.style.animation = 'none';
        }, 1000);
    }
}
