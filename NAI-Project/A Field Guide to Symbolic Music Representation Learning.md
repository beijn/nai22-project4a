\* best before next year


It can be downloaded and interactively explored and expanded from [here]()

This is a web of knowledge of state of the art (23/01) approaches to computational musicology with a focus on generative and neuro-symbolic systems. It can be navigated by clicking on the cross links (though most sadly remained placeholders) or #tags or by navigating the folder structure.  Each of the notes under 
- "Application Papers/" details a full recent paper, mainly following  the same structure (best to be discovered, see eg. [[ComMU]]).
- "Summaries and Conclusions/" tries to bring together related concepts from a higher point of view (like [[Music Evaluation Metrics]]) and draws overaching (sub-)conclusions (like [[Explainability vs Explain-Ability]]).
Most notes include a core sentence at the top, summarizing the central idea / value proposition. All notes include references.


- Relatively ugly material on relevant #symbolic and #neuro-symbolic approaches (mostly in the domain of language and abstract patterns) is to be found in "Checkpoint II.pdf".  This includes the [[Differential Neural Computer]] and [[VQ-VAE]](-II) architecturs. 
	- I did it for this course, but it hasn't made it into this final knowledge web, please see the [[A Field Guide to Symbolic Music Representation Learning#Checkpoint II|disclaimer below]].
- Entry material on human and AI #cocreativity (in the domain of images), including [[Meaningful Human Control]], [[Latent Space]] and [[VAE]] is to be found under "Previous Work/".
	- *It was for another course*, please see the [[A Field Guide to Symbolic Music Representation Learning#Previous Work on Human+AI Creativity|disclaimer below]].


### No stub notes and secondary literature
To streamline the presentation, concepts that are used only once are explained at that location (against the spirit of Obsidian).
Some secondary references, which were mentioned in the primary literature only with respect to one specifc concept and seemed of limited relevance to be read and understood have their citations been copied from the primary literature. 

## Libraries 
Besides the libraries that come with most of the presented papers there are highly usefull more general frameworks, that have not yet merrited an own entry. 
- Musicaiz [^@hernandez-olivanMusicaizPythonLibrary2022] is a recent attempt to provide a unified framework for *Symbolic Music Generation, Analysis and Visualization* by providing submodules for different common aspects and steps they identify when dealing with the topic of this work.  [source](https://github.com/carlosholivan/musicaiz) [docs](https://carlosholivan.github.io/musicaiz/index.html)
- 

- MidiTok
A Python library summarizing multiple methods to tokenize MIDI files for usage with sequential Deep Learning models like Transformers or Recurrent Neural Networks. Enables easy swapping between and fair comparison of tokenization methods.




## Related Work 
### Disclaimer on the scope of the presentation
I ran out of time. I have invested well over 70 hours, but struggling a long time to settle on a concrete plan, a big part of that was spent in blocks of different topics and research methodologies. Very interesting (though in volume much less) research in [[Evolutionary Algorithms]] has not been captured here, though it had a great impact on my interal idea space. Very unfortunately I havent managed, to transfer most of that work over to presentation in this work. This is because the process of converging on this presented format was very long and involved going over the same literature over and over. Most annoyingly it meant rereading a lot of material sometimes multiple times, as my demands on content detail expanded. Calculating with the required energy of improving the representation of recently read papers, that for completely redoing the work on previously read papers (Checkpoint II), the energy it gives me to read a new fascinating paper, and the pain of leaving too much previous work unused, I settled for this. This is a small set of overly work-intensive presentations of the most relevant recent computational musicology papers.

### Checkpoint II
In "Checkpoint II.pdf" several (less detailed and less accessible) reviews of papers relating to more #symbolic systems are collected. This includes recent work on the [[Abstract Reasoning Challange]], which provides state of the art neural, symbolic and hybrid approaches to complex patterned transformations aka reasoning. As detailed the MIR community (as of early 2023) has recently mainly focussed on adapting deep neural networks like [[Transformer]]s. The paper selection in Checkpoint II could therefore provide new research directions, especially the [[Differential Neural Computer]] contains untapped potential. Recent work on (re-)introducing #grammar based approaches to (simple) language modelling in *[[Learning Compositional Rules via Neural Program Synthesis]]*. 

### Previous Work on Human+AI Creativity 
The folder *Previous Work* includes course work done for *an other course*. It relates highly to my work here (as I realized in the end), but I weighted the benefit of doubling the work to copy it over into this knowledge web relatively low, while there were more prospectful candidates both for improvement and novel reading. **It is submitted to the benefit of comilitons, not to be graded as work for this course.** It is kindly recommended as an entry to the topic of Human and AI #cocreativity based on the concepts of navigation in [[Latent Space]], most accessible through the therin presented [[VAE]], and [[Meaningful Human Control]]

I have not managed to 

## Ethical Statements

### On the cultural bias of *Western* music
The author has not invested into expanding his horizon beyond western music tradition. The music which is targeted in the works picked up by this one is dominantly western. I stress that other kinds of music, coming with ways to systematize than wester #music-theory, must exist in the world and that the fact that it is so marginalized is a consequence of post colonialism. *This work likely takes part in reenforcing this marginalization, by reflecting work targeting specifically "western" music. Especially because not even glimpsing at other cultures. None less because it was uninented.* Science and innovation that narrow their gaze down to a specific culture, for whatever unscientific reason, directly contribute to reinforcing this culture's imperialism, through a multitude of obvious and less obvious ways. This holds especially when paired with economic interests, like a big part of contemporary research in AI music. 

### Human Work
This work was done by a human with limited AI assistance. Every presented article was read by me (for details on secondary references see above). AI was used only (mostly in form of TLDR;s and recommendations of related papers) through several mainstream literature websites like Semantic Scholar and Google Scholar.



[^@hernandez-olivanMusicaizPythonLibrary2022]: Hernandez-Olivan, Carlos, and Jose R. Beltran. 2022. “Musicaiz: A Python Library for Symbolic Music Generation, Analysis and Visualization.” [https://doi.org/grmp4f](https://doi.org/grmp4f).