A comprehensice 

- Transformers deal with 1-D sequences of tokens (drawn from a fixed vocabulary). This is not an intuitive representation for music, as the concept was developed without respect to time and the overlay of multiple interacting voices. 
- Furthermore (disregarding timbre, expression and so on, as most symbolic music models do) the structural difference between language tokens, from which there exists a huge number with relatively little systematicity, and music notes, which can be modeled relatively well (in some music stiles) as low dimensional combinations of low ranged features like pitch and volume, seems to need additional attention. 
- Various tokenization strategies (see [[MidiTok]][^@fradetMidiTokPythonPackage2021]) implement this separability of note features as chains of tokens of different types. Yet most NN applications to date don’t explicitly deal with the types, but treat all tokens in the same way as text tokens \[\[Compound Word Transformer]]. Instead of implementing an inductive bias of multiple of those tokens forming a discrete unit, this fact is implicitly to be learned by the attention mechanism. A very simple monophonous musical phrase thus already becomes a long sequence. Due to the quadratic time complexity of the (dot product) attention mechanism of transformers, this implies a heavy impediment on the length of processable sequences. Several strategies exist recently to address this inductive bias, detailed in the respective papers section . Also the sequence length becomes less impeding with the invention of linear time attention (see [[Linear Transformer]]).

((STRATEGIES FOR DEALING WITH THIS

*   Compound Word Transformer

))

nested processing? One system generates latent vectors for parts of a composition, so that they are linked, a subnet generates more low level latents from these and so on… Hirarchical Abstraction implemented as nested iterative latent expansion. Should also implement a mechanism for generated structures in lower levels to refer to similar substructures in sibling levels. In overall one wants a tree for hirarchical abstraction, but also interrelatedness for substructures depending on their latent relatedness atleast on the same level. And an iterative process of dialog between parts and levels until things agree / rough and random initial ideas have been polished.

2D transformer like ViT for music? pitch×time or per voice per time a pitch·velocity


## MidiTok 
### A python package for MIDI file tokenization [^@fradetMidiTokPythonPackage2021]
[source with great overview of all tokenization schemes](https://github.com/Natooz/MidiTok)

[TLDR] MidiTok is a Python package to encode MIDI files into sequences of tokens to be used with sequential Deep Learning models like Transformers or Recurrent Neural Networks to encode datasets with various strategies built around the idea that they share common parameters.

A Python library summarizing multiple methods to tokenize MIDI files for usage with sequential Deep Learning models like Transformers or Recurrent Neural Networks. Enables easy swapping between and fair comparison of tokenization methods.

[^@fradetMidiTokPythonPackage2021]: Nathan Fradet, Amal El Fallah Seghrouchni, Jean-Pierre Briot. 2021. “MidiTok: A Python Package for MIDI File Tokenization.” In _Extended Abstracts for the Late-Breaking Demo Session of the 22nd International Society for Music Information Retrieval Conference_.

