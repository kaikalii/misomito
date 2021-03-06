# Introduction

Misomito is a minimalist constructred spoken language.

It combines the simplicity of [Toki Pona](https://tokipona.org/) with the programatic formalism of [Lojban](https://mw.lojban.org/index.php?title=Lojban&setlang=en-US).

# Letters and Syllables

Misomito has 5 vowels and 6 consonants, but not all combinations are valid.

|     | K             | L      | M      | N         | S           | T           |
| --- | ------------- | ------ | ------ | --------- | ----------- | ----------- |
| A   | inteterminate | place  | or     | negative  |             | it          |
| E   | swap          | over   | rotate | drop      | dup         |             |
| I   | goodness      |        | person | alternate | time        |             |
| O   |               | action | and    | ownership | information | transaction |
| U   |               |        | many   |           |             | travel      |

# Roots

Misomito has 6 root words

## Mi - Person

Mi is any person. By default, it refers to the speaker.

## Ta - Thing

Ta is any animal or inanimate thing.

## La - Place

La is a place. By default, it refers to solid ground.

## Si - Time

Si is time. It can also mean life or existance.

## Ki - Goodness

Ki is goodness. It can refer to any thing that is considered good to the speaker, like love, warmth, food, etc.

## So - Information

So is information.

# Functions

Misomito has 14 function words. These words pop/push other items from/to the stack.

## No, To, and Tu - Relationships

No, To, and Tu all pop either 2 or 3 items from the stack and may push a single item back.

### No - Ownership

No pops two items from the stack, indicates that the lower item owns the higher item. By default, it pushes the owned item back onto the stack. If the owner is a ka item, its ka is removed, and it is pushed instead.

### Tu - Travel

Tu pops two items from the stack and indicates that the lower item "moves to" the higher item. This can mean literal travel or something more abstract, like a state change. If either of the items is a ka item, its ka is removed, and it is pushed onto the stack.

### To - Transactions

To pops three items from the stack and indicates that the middle item "moves" from the lowest item to the highest item. This can mean literal travel or something more abstract. If any of the items is a ka item, its ka is removed, and it is pushed onto the stack.

## Na and Ni - Adjacent concepts

Na and Ni both pop a single item from the stack and push an item that has an adjacent concept.

Na is typically a negation, while Ni usually indicates some different but relates item.

### Mi

- mina - someone who is not me (defaults to same gender as speaker)
- mini - you
- minani - someone who is not me and is the opposite gender from me

### La

- lana - sky/air/gas/space
- lani - water/ocean/liquid

### Si

- sina - never

### Ki

- kina - badness

## Ma and Mo - Logical set builders

Ma and Mo both pop two items from the stack and build a logical set.

### Mo - And

Ma groups two items together.

"A B mo" means A and B.

"A B C mo mo" means A, B, and C.

### Ma - Or

Mo creates the inclusive-or set of two items.

"A B ma" means A or B.

"A B ma ma" means A, B, or C.

## Ka - Interterminate

Ka indicates that the item on the top of the stack is indeterminate. This can be used either to ask a question or to make an item more indeterminate than another when using a relationship function (no, to, or tu).

mi so mi**ka** to => Who do I talk to?

mi**ka** so mi to => Who is talking to me?

mi**ka** ki mi to => My friend (literally, the person who gives goodness to me)

## Mu - Many

Mu indicates that there is more than one of something. When followed by Ka, it asks how many or indicates an amount.

mi so**mu** no => I know many things.

mi ta**mu**ka mini to => How many should I give you?

mi mi ta**mu**ka no mini to => I gave you everything I have.

## Ke, Le, Ne, and Se - Stack Manipulation

Ke, Le, Ne, and Se have no actual meaning on their own. They only manipulate the stack.

### Se - Duplicate

Se duplicates the item on the top of the stack.

mi **se** mi tu => I am staying where I am.

**se** ta no => It is his.

### Ke - Swap

Se swaps the two items on top of the stack.

mikakimito se somu no. mi **ke** tu. => My friend is smart. I am meeting him.

### Le - Over

Le copies the second item from the top of the stack to the top of the stack.

mi mini **le** **le** ke no no => I am yours. You are mine.

### Me - Rotate

Me removes the third item in the stack and pushes it to the top.

mikakimito mi so **me** to => I talk to my friend.

### Ne - Drop

Ne pops an item from the top of the stack and pushes nothing.

minisono se kika no. **ne** kinaka no. => Are you happy? Are you sad?

The first no pushes ki onto the stack. However, we want to refer to minisono again, so we use ne to pop kika.

# Lo

Lo is a special word that does not pop directly from the stack.

Lo pushes that relationship created by the most recently used no, to, or tu (rather than one of its components) onto the stack.

_minaka_ ta mi to. ki mi to. => I like the _person_ who gives it to me.

mina _taka_ mi to. ki mi to. => I like the _thing_ they give to me.

mina ta mi to. **lo** ki mi to. => I like **that** they give it to me.
