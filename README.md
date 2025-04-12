## Ejercicio 7

```
//Mixin básico

mixin Volar {
  void volar() {
    print("Puedo Volar");
  }
}

mixin Acelerar {
  void acelerar() {
    print("Puedo Acelerar");
  }
}

mixin Navegar {
  void navegar() {
    print("Puedo Navegar");
  }
}

class Avion with Volar, Acelerar {
  void mostrar() {
    print("Soy un Avion");
  }
}

class Bote with Navegar, Acelerar {
  void mostrar() {
    print("Soy un Bote");
  }
}

class Auto with Acelerar {
  void mostrar() {
    print("Soy un Auto");
  }
}

void main() {
  Avion av = Avion();
  av.mostrar();
  av.volar();
  av.acelerar();
  
  Bote bo = Bote();
  bo.mostrar();
  bo.acelerar();
  bo.navegar();
  
  Auto au = Auto();
  au.mostrar();
  au.acelerar();
}
```

## Ejercicio 8

```
//Mixin básico

mixin Curar {
  void curar() {
    print("curar");
  }
}

mixin Armas {
  void armas() {
    print("pelear con armas");
  }
}

mixin Hechizo {
  void hechizo() {
    print("Lanzar hechizo");
  }
}

class Mago with Hechizo, Curar {
  void mostrar() {
    print("Soy un Mago estas son mis habilidades:");
  }
}


void main() {
  Mago av = Mago();
  av.mostrar();
  av.curar();
  av.hechizo();
}

```
