# Portfólio ((Em construção))
Meu portfólio utilizando apenas CSS e Html

/*
/*  TESTANDO CARROSSEL*/

.carousel {
  /*width: 50%;*/
  padding: 20px 0;
  overflow: hidden;
  background-color: #51e765;
}

.card {
  
  color: white;
  border-radius: 24px;
  box-shadow: rgba(0, 0, 0, 10%) 5px 5px 20px 0;
  /*padding: 20px;*/
  font-size: xx-large;
  justify-content: center;
  align-items: center;
  /*min-height: 200px;*/
}

.card img{
  width: 300px;
  height: 350px;
}

.carousel {
  /* ... */
  > * {
    flex: 0 0 0;
  }
}

/* Agrupe os cartões para melhorar a estrutura. */
.group {
  display: flex;
  gap: 20px;
  /* Adicione padding à direita para criar um espaço entre o último e o primeiro cartão. */
  padding-right: 20px;
}
.group {
  /* ... */
  will-change: transform; /* Devemos ser gentis com o navegador - informar o que vamos animar. */
  animation: scrolling 30S linear infinite;
}

@keyframes scrolling {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-100%);
  }
}
.carousel {
  /* ... */
  &:hover .group {
    animation-play-state: paused;
  }
}



