# Projeto-Alice

# WIKI do Trabalho: Animação Alice 3 (Orientação a Objetos)

**Aluno:** Felipe Mendes Campos
**RA:** 10740655

---

## 1) Storyboard
*<img width="735" height="1000" alt="image" src="https://github.com/user-attachments/assets/6dfe70ef-1e3f-4f32-815e-c3d912d362b3" />
*

**Resumo das Cenas:**
* **Cenas 1 e 2:** As irmãs de Blue recebem alimento da mãe, um por vez.
* **Cena 3:** Blue não recebe comida.
* **Cena 4:** Blue se revolta e diz: "Cansei disto, vou ser independente".
* **Cena 5:** Blue pula do ninho.
* **Cena 6:** Blue está caindo.
* **Cena 7:** Blue cai contra o chão.
* **Cena 8:** Blue levanta-se e, com asas abertas, diz: "Finalmente sou livre".
* **Cena 9:** Gavião pega Blue.
* **Cena 10 (Bad Ending):** No céu, o gavião diz: "Finalmente comida fácil kkkkk".

---

## 2) Planejamento da Implementação (Algoritmo)

**Configuração (Setup):**
* **Cenário:** Natureza (Ground, japaneseCypress9).
* **Objetos (Instâncias):** araraMae, irma1, irma2, blue (da classe de Pássaros) e gaviao.

**Sequência Lógica (myFirstMethod):**
1. **doInOrder** (Alimentação)
   * araraMae vira para irma1 e simula entrega de comida (move down/up).
   * araraMae vira para irma2 e simula entrega de comida.
2. **doInOrder** (Revolta e Pulo)
   * blue vira para araraMae (opcional).
   * blue diz "Cansei disto, vou ser independente".
   * blue move forward.
3. **doTogether** (Queda sincronizada)
   * blue move down (até o chão).
   * camera move down (acompanhando).
4. **doInOrder** (A Captura)
   * blue diz "Finalmente sou livre".
   * gaviao vira para blue.
   * gaviao move to blue.
   * blue define gaviao como veículo (setVehicle).
5. **doTogether** (Fim)
   * gaviao move up (levando blue junto).
   * camera move up.
   * gaviao diz "Finalmente comida fácil kkkkk".

---

## 3) Arquivo do Projeto Alice
projeto esta no repositório
---

## 4) Vídeo Explicativo - Conceitos de POO
* **Link:** https://youtu.be/KIPOmCb8g7c

* 
**Conceitos demonstrados no vídeo:**
* **Classe:** O molde usado na galeria do Alice para criar as aves.
* **Objeto/Instância:** Os personagens na tela (ex: o 'blue' e o 'gaviao').
* **Atributos:** As propriedades (cor, tamanho) que diferenciam o 'blue' das irmãs.
* **Métodos:** As ações executadas e nativas (say, move, turnToFace, setVehicle).
* **Estruturas de Controle:** O uso de `doInOrder` para sequenciamento e `doTogether` para concorrência (como na cena da queda).
