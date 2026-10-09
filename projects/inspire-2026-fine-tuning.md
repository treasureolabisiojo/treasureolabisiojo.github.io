# Teaching a Language Model to Sort Consumer Complaints

- **One-line summary:** I fine-tuned a small open language model to sort real consumer
  complaints into six categories, then trained it across multiple GPU nodes on a
  supercomputer to measure the speedup.
- **When:** October 2026
- **Where / program:** INSPIRE 2026 student workshop, Austin, Texas
- **My role:** (solo in the morning; in the afternoon my team role was Driver / Recorder / Skeptic / Reporter)
- **Tools:** Python, Jupyter, Hugging Face Transformers, LoRA (PEFT), the Vista GPU supercomputer

## The problem

The CFPB Consumer Complaint Database holds millions of complaints from the public.
Someone has to sort each one (credit reporting, debt collection, mortgage, credit card,
bank account, and more). Can a small AI model learn to do it?

## What I did

1. Explored real complaints and guessed which categories would be hard to tell apart.
2. Scored the untrained model: about 17%, which is chance for six categories.
3. Fine-tuned it with LoRA on a GPU and scored it again.
4. Wrote my own complaints to try to trick it.
5. With my team, ran the same training on 1, 2, and 4 nodes and measured the speedup.

## Results

- Accuracy before training: about 17%
- Accuracy after training: ____%
- Seconds to train on one GPU: ____
- Time on 1 node: ____ · on 4 nodes: ____ · speedup: ____x

## What I learned

(One or two sentences. What surprised you?)

## Images

- `images/...` : (a screenshot of your results or your team's scaling chart)

## Links

- Workshop code: https://github.com/ashleyscruse/hpc-finetune-workshop
