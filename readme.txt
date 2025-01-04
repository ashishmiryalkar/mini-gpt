Mini gpt This implementation presents a complete decoder-only transformer network,
inspired by the GPT-2 architecture. It is designed as a smaller-scale version of GPT-2,
featuring a reduced embedding dimension of 768 and a context length of 256.
These modifications result in a more compact model with lower computational requirements,
while still retaining the fundamental transformer architecture."

The code is divided into three parts

Part 1: Attention
    Various Attention models are implemented from scratch
        self Attention
        Casual Attention
        Multihead Attention
        Masked Multihead Attention
        Efficient Multihead Attention.

Part 2: Transformer Decoded (GPT 2)
    Complete implementation of a transformer block which contains
        Layer normalization
        Activation Function (GELU)
        Feed Forward Network.

    A complete GPT 2 model is created and showed the number of learnable parameters are equal to 124million ( gpt-small )

Part 3: Training and Inference.
    Data set loader and dataset preperation using pytorch.
    creating datasets for Training and Validation.
    Loss calculation implementation using cross entropy.
    Function to predict the next tokens and decoding the tokens.
    greedy retrival and Multinomial retrival of tokens from the logits.
    Temperature scaling of the model logits.
    Training the model.
    Validating the model.
    Generating text from the data.

References : Build a Large Language Model ( from scratch ) - sebastian Raschaka.