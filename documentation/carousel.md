# Carousel

Cette composante permet d'instancier un carousel sur un élément html.

<br><br>

# Dépendance

### Swiper

Afin d'utiliser cette composante, vous devrez vous assurer que Swiper soit installé dans votre projet.

`npm install swiper`

<br><br>

# Comment l'utiliser

### **HTML**

Afin d'utiliser la composante, mettre l'attribut **data-component="Carousel"** sur une structure html respectant celle de la librairie Swiper.

```
<div class="swiper-container" data-component="Carousel">
```

<details>
<summary>Exemple complet</summary>

```
<!-- Slider main container -->
<div class="swiper-container" data-component="Carousel">
  <!-- Additional required wrapper -->
  <div class="swiper-wrapper">
    <!-- Slides -->
    <div class="swiper-slide">Slide 1</div>
    <div class="swiper-slide">Slide 2</div>
  </div>
  <!-- If we need pagination -->
  <div class="swiper-pagination"></div>
</div>
```

</details>

<br><br>

### **SCSS**

Pour que les styles soient bien appliqués, il faut importer les styles de bases de Swiper.

```
@import '../../node_modules/swiper/swiper.scss';

// seulement si vous avez des options supplémentaire comme la pagination
@import '../../node_modules/swiper/components/pagination/pagination.scss';

```

Voir la [Documentation complète de Swiper](https://swiperjs.com/swiper-api)

<br><br>

# Variantes

<br>

### **DÉFAUT**

Cette variante permet d'avoir une _slide_ à la fois dans tous les résolutions d'écran.

_Elle ne requiert aucune configuration supplémentaire._

<br>

### **SPLIT**

Cette variante permet d'avoir 2 _slides_ du carousel visible en simultanné sur grand écran (1024px et plus), mais seulement une _slide_ sur écran plus petit (1023px et moins). Pour activer cette variante, il faut ajouter sur votre component l'attribut suivant:

### **HTML**

```
data-carousel="split"
```

<details>
<summary>Exemple complet</summary>

```
<!-- Slider main container -->
<div class="swiper-container" data-component="Carousel" data-carousel="split">
  <!-- Additional required wrapper -->
  <div class="swiper-wrapper">
    <!-- Slides -->
    <div class="swiper-slide">Slide 1</div>
    <div class="swiper-slide">Slide 2</div>
  </div>
  <!-- If we need pagination -->
  <div class="swiper-pagination"></div>
</div>
```

</details>

<br><br>

# Crédit

Cette librairie est une création de Jean-François Leblanc et Matthieu Parent, pour le département TIM du Cégep édouard Montpetit.

Elle a été modifié par [votre_nom](https://dectim.ca/)
