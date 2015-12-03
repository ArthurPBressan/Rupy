RuPy
====
(Designa)

### Patrocinadores
* Toptal
* ZNC

Python Brasil 2015: Prêmios em dinheiro. R$ 3k para distribuir para contribuições + commits aceitos.

Freelancer Lifestyle
=====================
Palestrante: Henrique Bastos 

Google +, LinkedIn, Facebook

Falta:

* Dinheiro

* Tempo

* Dinheiro

* Coragem 

Disclaimer: **Viajem da cabeça, não drogas: Oferta**


Nós nascemos on Rails: Nós somos usados pelo *sistema*.
O *sistema* usa as pessoas como insumo.


A aventura é busca por autonomia:

**Autonomia**:

* Ser burro por conta própria.

* **Não** é *independência*.

Bolha .com -> jovens não queriam ir para grandes empresas -> Startups de hoje.

Rede: Pontencial de interconexão de todos os indivíduos.

**Colaboração** > Competição:
Vídeo: History of Python (Time-lapse do repositório de Aug 1990 -> Junho 2012)
Link: Steve Albini @ Face The Music 2014 (Youtube)

Crise do intermediário: Bom para a Autonomia

* Sistema Empurrado:
	* Ancorado na dependência.
	* Sempre subordinado a alguém ou empresa.

* Sistema Puxado:
	* Faz o que precisa ser feito. 
	* Sistema que aceita prioridade.
	* Aceita limitações.

*Temos que ir do empurrado para o puxado*


Tempo e Eficácia > Volume e Eficiência


*Sujeito Objeto:*
Sujeito quem faz ação.
Objeto o que a ação se aplica.
Temos que ver se somos sujeitos ou objetos.


*Entender o tempo:*

* Livro: Sílvio Meira - O futuro vem do futuro.

* Tédio: Falta alguém mandando.

* The Way We're Working Isn't Working: Administre energia, não o tempo.


Autonomia: Relação de igual com o mundo.

* Livro: O que o medo pode nos ensinar - Karen Thompson Walker.

* *Fear is the path to the dark side*.

* Medo do não: 100% dos problemas é por não dizer não.

* Plantinha do foda-se: Plante e distribua.


Início: Para dentro e para frente.

* E*u*preendedorismo

* Quadrante dos talentos:
	* Gosta mas não sabe
		* Venda barato
	* Não gosta e não sabe
		* Cuidado ao delegar
	* Gosta e sabe fazer bem
		* Abraço
	* Não gosta mas sabe fazer bem
		* Cobrar caro


**S.M.A.R.T.: Boas metas**

* Specific (Simples e direto)

* Measurable (Quanto)

* Attributable (Quem)

* Realistic

* Temporal


**Dinheiro:**

* Mapear receita (Líquido):
	* FGTS é do governo.
	
* Mapear despesas (Varáveis e Fixas):
	* Gastar menos do que ganha
	
* Valores não em reais mas em horas

* *"Seja frugal"*:
	* Consumo ou investimento
	
* Autonomia de voo:
	* Fluxo de caixa anual 
	* Não quanto tem, mas quanto precisa
	
* Dinheiro tem preço:
	* Dívida de cartão/cheque especial: Fodeu.
	
* Múltiplas Linhas de Receita

* Rentabilidade > Faturamento


Programador: 
* Não é transformar café em código

* Gerar experiẽncia que transforme melhore a vida de alguém.

*Vender vender vender:*
* Nerdcast com Shoptime.

* Livro: To Sell is Human - Daniel H. Pink.

* Serviço/Solução. 

* Livro: Como Fazer Amigos e Influenciar Pessoas - Dale Carnegie

* Transparência:
	* Nada é mais caro do que vender para quem não é seu cliente
	
* Preço:
	```python
		i_want = set(range(my_min, my_max))
		client_wants = set(range(min, max))
	```
	
* CLT é mais fácil:
	* Corporação: Reunião de corpos.
	
	* Empresa é um papel.
	
	* PJ: Responsabilidade limitada.



Python Birds
============
GitHub: pythonprobr/pythonbirds

Palestrante: Renzo Nuccitelli
renzo@python.pro.br

Eduardo Guerra: Editor Mundo J

Python para Zumbis


Turma Alpha:
* 12 horas para terminar o jogo:
* Com replay deixava complicado

Turma Beta:
* Conseguiu terminar

Instalação no linux:
sudo apt-get install python3-tkinter

TDD:
* Testes já prontos.

Conclusões:
* Foco no Cliente (Alunos)
* Rede de Contatos
* **PESSOAS, PESSOAS, PESSOAS**
	* Tecnologia não é o problema.

www.python.pro.br


-----------------------------------------
Livro: Invent Your Own Games With Python (.pdf)
Livro: Python for Kids


Projeto Decolar (CAED):

* Ensino de várias matérias (Química, Física, etc.) para crianças

* Voluntário
 
Automação com Python - pingo: pingo.io - Garoa HC


Programação Funcional & Concorrência - Elixir
=============================================
Palestrante: Roberto Pepato

**Por que programação funcional:**

* bit.ly/freelunchisover

* Desenvolvedor sem skill multicore: Caindo fora do mercado.

**Elixir:**

* Livro: Structure and Interpretaion of Computer Programs. (Lisp)

* Erlang

* IoT

* Livro: Programming Elixir - Dave Thomas

**Don't** Move Forward unless you accept that:

* OO não é o único jeito.
etc.

Pattern Matching:

* "=" é diferente.
	* ~~Atribuição~~ 
	* Asserção (match)

Tutorial de Elixir:

* Imutabilidade dos dados

* Função com múltiplos corpos
	* Exceções
	
* Funções retornam funções

* &: Shorthand para funções

* Módulos

* Pipe (**|>**)
	* Syntact sugar
	* Fluxo de execução: Perto da especificação
	
* Listas e recursão
	* Listas podem ser vazias, ou consiste de uma cabeça e cauda. A cabeça é um valor e o resto é uma lista
	
	* "Itera" recursivamente
	
	* Exemplos:
		* Comprimento: Uma lista vazia == 0, não vazia == 1 + comprimento da cauda.
		
		* Map: Passa uma lista e uma função qualquer 


FizzBuzz:
```elixir
fb.exs

defmodule FizzBuzz do
	def fb_term do
		fn
			(0, 0, _) -> "FizzBuzz"
			(0, _, _) -> "Fizz"
			(_, 0, _) -> "Buzz"
			(_, _, c) -> c
		end
	end

	def of(n) do
		fb_term.(rem(n, 3), rem(n, 5), n)
	end

	def upto(n) do
		...
	end
end
```
