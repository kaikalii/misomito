# Letters and Syllables

Misomito has 5 vowels and 6 syllables, but not all combinations are valid.

|     | K             | L     | M      | N         | S           | T           |
| --- | ------------- | ----- | ------ | --------- | ----------- | ----------- |
| A   | inteterminate | place | or     | negative  |             | it          |
| E   | swap          | over  |        | drop      | dup         |             |
| I   | goodness      |       | person | alternate | time        |             |
| O   |               |       | and    | ownership | information | transaction |
| U   |               |       | many   |           |             | travel      |

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

Misomito has 13 function words. These words pop/push other items from/to the stack.

## No, To, and Tu - Relationships

No, To, and Tu all pop either 2 or 3 items from the stack and push a single item back.

### No - Ownership

"A B no" means A owns B and pushes the owned item onto the stack. Ownership can mean literal ownership, as in a person's possesions, or it can mean in or on something.

### Tu - Travel

"A B tu" means A goes to or travels to B and pushes the less determinate items onto the stack.

### To - Transactions

"A B C to" means B goes from A to B and pushes the least determinate item onto the stack. This usually means the exchange of an item from one entity to another. This can also mean travel from a start to an end.

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

mika ki mi to se somu no. mi **ke** tu. => My friend is smart. I am meeting him.

### Le - Over

Le copies the second item from the top of the stack to the top of the stack.

mi mini **le** **le** ke no no => I am yours. You are mine.

# Determinacy

No, To and Tu push onto the stack the modified input that is least determinate.

Root words have a base indeterminacy, while function words modify it.

| Indeterminacy | Roots          |
| ------------- | -------------- |
| 1             | mi             |
| 2             | ki             |
| 3             | ta, la, si, so |

Some function words increase the indeterminacy of an item.

| Words           | Indeterminacy |
| --------------- | ------------- |
| ka              | +10           |
| na (on mi item) | +3            |
| everything else | +0            |

## Examples

In these examples, the least determinate term is in bold.

**mina** ki mi to => pushes "my friend" (literally "the person who gives goodness to me") onto the stack

mina **kika** mi to => pushes "the goodness they give me" onto the stack

mina ki **minaka** => pushes "his friend" (literally "the person he gives goodness to") onto the stack.

la **mina** no => The person who is at the place (The place owns the person)

**mina** la no => The person who owns the place (The person owns the place)

**laka** mina no => The place where the person is (The place owns the person)

mina **laka** no => THe place the person owns (The person owns the place)
