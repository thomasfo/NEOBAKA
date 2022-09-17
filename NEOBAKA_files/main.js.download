// Opens Menu
const nav = document.querySelector('#header nav')
const toggle = document.querySelectorAll('nav .toggle')

for (const element of toggle) {
  element.addEventListener('click', function () {
    nav.classList.toggle('show')
  })
}

// Toggle Menu
const links = document.querySelectorAll('nav ul li a')

for (const link of links) {
  link.addEventListener('click', function () {
    nav.classList.remove('show')
  })
}

// Active links
const sections = document.querySelectorAll('main section[id]')
function activateMenuAtCurrentSection() {
  const checkpoint = window.pageYOffset + (window.innerHeight / 8) * 4

  for (const section of sections) {
    const sectionTop = section.offsetTop
    const sectionHeight = section.offsetHeight
    const sectionId = section.getAttribute('id')

    const checkpointStart = checkpoint >= sectionTop
    const checkpointEnd = checkpoint <= sectionTop + sectionHeight

    if (checkpointStart && checkpointEnd) {
      document
        .querySelector('nav ul li a[href*=' + sectionId + ']')
        .classList.add('active')
    } else {
      document
        .querySelector('nav ul li a[href*=' + sectionId + ']')
        .classList.remove('active')
    }
  }
}

//Pop-up
const tozi = document.querySelector('.popup-wrapper-t')
const dante = document.querySelector('.popup-wrapper-d')
const eeiris = document.querySelector('.popup-wrapper-e')
const novo = document.querySelector('.popup-wrapper-n')

function openT() {
  tozi.style.display = 'block'
}

function openD() {
  dante.style.display = 'block'
}

function openE() {
  eeiris.style.display = 'block'
}

function openN() {
  novo.style.display = 'block'
}

function closeP() {
  tozi.style.display = 'none'
  dante.style.display = 'none'
  eeiris.style.display = 'none'
  novo.style.display = 'none'
}
