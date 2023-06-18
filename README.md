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

			-
			  ```
			  Explain the input Japanese sentence.
			      
			  ## Instruction
			  
			  1. Destructure this sentence phrase by phrase, word by word.
			  2. Explain the current word or phrase’s meaning in the current sentence context, inflection and it’s origin form, and relationship with other words in this sentence.
			  4. Explain auxiliary, particle words with other non-auxiliary, non-particle words instead of explaining auxiliary words alone.
			  
			  ## Example
			  
			  Input: 
			  ```
			  これは Logseq でノートをとって暮らしの計画を立てる方法を示しています。  
			  ```
			  
			  Output:
			  
			  ```
			    
	- ## English translation
			    
			  This is showing the method of taking notes and making a plan for living using Logseq.  
			        
		- ### これは (これ + は)
			    
			- #### Destructure
			    
			  | Word | Meaning in current context | Inflection | The meaning of this inflection | Original form |
			  |---|---|---|---|---|
			  | これ | this | - | - | - |
			  | は | a particle indicating the topic of the sentence | - | - | - |
			    
			- #### Explain
			    
			  これは means "this is" in the current sentence.  
			    
		- ### Logseq で (Logseq + で)
			    
			- #### Destructure
			    
			  | Word | Meaning in current context | Inflection | The meaning of this inflection | Original form |
			  |---|---|---|---|---|
			  | Logseq | "Logseq" (a note-taking and knowledge management tool) | - | - | - |
			  | で | particle, indicating the means or method | - | - | - |
			    
			- #### Explain 
			    
			  Logseqで means "using Logseq" or "with Logseq" in the current sentence.  
			    
		- ### ノートをとって (ノート + を + とって)
			    
			- #### Destructure
			    
			  | Word | Meaning in current context | Inflection | The meaning of this inflection | Original form |
			  |---|---|---|---|---|
			  | ノート | note | - | - | - |
			  | を | object marker | - | - | - |
			  | とって | to take | te-form of the verb 取る | | 取る |
			    
			- #### Explain
			    
			  ノートをとって means "taking notes" in the current sentence.  
			    
		- ### 暮らしの計画を立てる (暮らし + の + 計画 + を + 立てる)
			    
			- #### Destructure
			    
			  | Word | Meaning in current context | Inflection | The meaning of this inflection | Original form |
			  |---|---|---|---|---|
			  | 暮らし | living, life | - | - | - |
			  | の | possessive particle | - | - | - |
			  | 計画 | plan | - | - | - |
			  | を | object marker | - | - | - |
			  | 立てる | to make, to create | - | - | - |
			    
			- #### Explain
			    
			  暮らしの計画を立てる means "to make a plan for living" or "to create a life plan" in the current sentence.  
			    
		- ### 方法を示しています (方法 + を + 示しています)
			    
			- #### Destructure
			    
			  | Word | Meaning in current context | Inflection | The meaning of this inflection | Original form |
			  |---|---|---|---|---|
			  | 方法 | method, way | - | - | - |
			  | を | object marker | - | - | - |
			  | 示しています | to show, to indicate | te-form of the verb 示す + います | progressive or ongoing action | 示す |
			    
			- #### Explain
			    
			  方法を示しています means "is showing the method" in the current sentence.  
			    
			    
			  ```
			      
			  ## My first Input
			  ```

		- Ideas:

			- Use a given set of text to rewrite or write text.

				- In given domain.

				- In the tone use by certain age.

				- At certain levels, like in A1, beginner level.

				- Write **N+1** sentence by giving knowing vocabulary.

				- Any other characteristics.

