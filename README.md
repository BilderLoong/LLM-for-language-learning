- Usage

	- Use LLM as an smart dictionary,

		- Use case：

			- Make the LLM consider the context to choose the right meaning of the word in current context.

			- Explain the word's etymology between two similar languages, e.g.: Japanese and Chinese; French and English.

			- Explain the inflection of the words, the meaning of this inflection, and why use this inflection in the current context.

			-

	- Ask LLM to generate immersion materials:

		- Prompt:

			-
			  ```
			  Write a story in target_language to help me learn the target_language.
			  
			  My target_language is: French.
			  
			  ## Instruction
			  - The story should be simple, short, and easy to understand.
			  - Each sentence should be less than 10 words.
			  - Add Japanese translation sentence by sentence along with the target_language.
			  - Choose words used most often in target_language.
			  - {Explain}: Explain the target_language sentence word by word, phrase by phrase.
			  	- {Explain} format: {target_language word} (*{English word}*)
			      	- Example for {Explain}: Elle (*She*) a (*has*) un vélo (*a bike*) rouge (*red*).
			  
			  ## Output Format
			  {target_language}
			  - 日本語: {日本語}
			  - Explain: {Explain}
			  ```

		- Ideas:

			- Use a given set of text to rewrite or write text.

				- In given domain.

				- In the tone use by certain age.

				- At certain levels, like in A1, beginner level.

				- Write **N+1** sentence by giving knowing vocabulary.

				- Any other characteristics.

