# Comparing `tmp/haloop-0.0.5.tar.gz` & `tmp/haloop-0.0.6.tar.gz`

## Comparing `haloop-0.0.5.tar` & `haloop-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/beam.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/ctc.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/data.py
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/loop.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/model.py
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/rnnlm.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/star.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/symbol_tape.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/transducer.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 haloop-0.0.5/ha/xen.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 haloop-0.0.5/.gitignore
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 haloop-0.0.5/README.md
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 haloop-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 haloop-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/beam.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/ctc.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/data.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/loop.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/model.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/resnet.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/rnnlm.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/scan.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/star.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/symbol_tape.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/transducer.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/xen.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.6/LICENSE
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 haloop-0.0.6/README.md
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 haloop-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 haloop-0.0.6/PKG-INFO
```

### Comparing `haloop-0.0.5/.github/workflows/release.yml` & `haloop-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `haloop-0.0.5/ha/beam.py` & `haloop-0.0.6/ha/beam.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.5/ha/ctc.py` & `haloop-0.0.6/ha/ctc.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.5/ha/data.py` & `haloop-0.0.6/ha/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def make_frames(wav):
     frames = torchaudio.compliance.kaldi.mfcc(wav)
 
     # frames = torchaudio.compliance.kaldi.fbank(wav, num_mel_bins=80)
     # frames += 8.
     # frames /= 4.
-    return frames
+    return frames # (T, F)
 
 
 class Directory(torch.utils.data.Dataset):
     def __init__(self, path: Path):
         super().__init__()
         self.files = list(path.glob("*.wav"))
 
@@ -37,14 +37,44 @@
         return len(self.librispeech)
 
     def __getitem__(self, index):
         wav, sr, text, speaker_id, chapter_id, utterance_id = self.librispeech[index]
         return make_frames(wav), text
 
 
+class Mask(torch.utils.data.Dataset):
+    def __init__(self, dataset):
+        super().__init__()
+        self.dataset = dataset
+
+    def __len__(self):
+        return len(self.dataset)
+
+    def __getitem__(self, index):
+        frames, text = self.dataset[index]
+
+        frames = frames[None,None,:]
+
+        frames = torchaudio.functional.mask_along_axis_iid(
+            frames,
+            mask_param=2, # mask a little bit as we have only 13 components
+            mask_value=0,
+            axis=3 # frequency
+        )
+
+        frames = torchaudio.functional.mask_along_axis_iid(
+            frames,
+            mask_param=7,
+            mask_value=0,   
+            axis=2 # time
+        )
+
+        return frames[0, 0, :], text
+
+
 class WordDrop(torch.utils.data.Dataset):
     def __init__(self, dataset, p_drop_words=0.4):
         super().__init__()
         self.dataset = dataset
         self.p_drop_words = p_drop_words
 
     def __len__(self):
@@ -68,14 +98,16 @@
             return LibriSpeech(subset)
         case ['head', subset]:
             return torch.utils.data.Subset(LibriSpeech(subset), range(16))
         case ['wdrop.4', subset]:
             return WordDrop(make_dataset(subset), p_drop_words=0.4)
         case ['wdrop.1', subset]:
             return WordDrop(make_dataset(subset), p_drop_words=0.1)
+        case ['mask', subset]:
+            return Mask(make_dataset(subset))
 
 
 def concat_datasets(s):
     if not s:
         return []
     parts = s.split(',')
     paths = [Path(part) for part in parts]
```

### Comparing `haloop-0.0.5/ha/loop.py` & `haloop-0.0.6/ha/loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 import torch.utils.data
 from kaldialign import edit_distance, align
 import wandb
 
 from .data import concat_datasets
 from .beam import ctc_beam_search_decode_logits
 from .model import Encoder, CTCRecognizer, StarRecognizer
+from .resnet import FixupResNet, FixupBasicBlock
 from .xen import Vocabulary
+from . import symbol_tape
 
 
 console = Console()
 def print(*args, flush=False, **kwargs):
     console.log(*args, **kwargs)
 
+
 class Collator:
     def __init__(self, vocabulary):
         self.vocabulary = vocabulary
 
     def __call__(self, batch):
         input_lengths = torch.tensor([len(b[0]) for b in batch])
         inputs = torch.nn.utils.rnn.pad_sequence([b[0] for b in batch], batch_first=True)
@@ -33,36 +36,53 @@
         return inputs, targets, input_lengths, target_lengths
 
 
 class System(nn.Module):
     def __init__(self, args):
         super().__init__()
         self.args = args
-        self.encoder = Encoder().to(args.device)
-        self.vocabulary = Vocabulary(args.glottal_closures)
-        if args.star_penalty is not None:
-            self.recognizer = StarRecognizer(star_penalty=args.star_penalty,
-                                             vocab_size=len(self.vocabulary)).to(args.device)
-        else:
-            self.recognizer = CTCRecognizer(vocab_size=len(self.vocabulary)).to(args.device)
+
+        match args.encoder:
+            case "lstm":
+                self.encoder = Encoder().to(args.device)
+            case "r9":
+                self.encoder = FixupResNet(FixupBasicBlock, [5,5,5]).to(args.device)
+
+        match args.vocab:
+            case "bytes":
+                self.vocab = symbol_tape.Vocabulary.bytes()
+            case "cmu":
+                self.vocab = Vocabulary(add_closures=False)
+            case "xen":
+                self.vocab = Vocabulary(add_closures=True)
+
+        match args.star_penalty:
+            case None:
+                self.recognizer = CTCRecognizer(vocab_size=len(self.vocab)).to(args.device)
+            case star_penalty:
+                self.recognizer = StarRecognizer(star_penalty=star_penalty,
+                                                 vocab_size=len(self.vocab)).to(args.device)    
+
         self.optimizer = torch.optim.Adam(chain(self.encoder.parameters(), self.recognizer.parameters()), lr=args.lr)
         self.scaler = torch.cuda.amp.GradScaler()
 
     def load_state_dict(self, checkpoint):
         self.encoder.load_state_dict(checkpoint['encoder'])
         self.recognizer.load_state_dict(checkpoint['recognizer'])
         self.scaler.load_state_dict(checkpoint['scaler'])
         self.optimizer.load_state_dict(checkpoint['optimizer'])
+        self.vocab.load_state_dict(checkpoint['vocab'])
 
-    def state_dict(self, **extra):
+    def make_state_dict(self, **extra):
         return {
             'encoder': self.encoder.state_dict(),
             'recognizer': self.recognizer.state_dict(),
             'scaler': self.scaler.state_dict(),
             'optimizer': self.optimizer.state_dict(),
+            'vocab': self.vocab.state_dict(),
         } | extra
 
     def train_one_epoch(self, epoch, train_loader):
         args, device = self.args, self.args.device
         encoder, recognizer, optimizer, scaler = self.encoder, self.recognizer, self.optimizer, self.scaler
 
         optimizer.zero_grad()
@@ -73,14 +93,16 @@
         t0 = time.time()
         for i, (inputs, targets, input_lengths, target_lengths) in enumerate(train_loader):
             inputs = inputs.to(device)
             targets = targets.to(device)
             input_lengths = input_lengths.to(device)
             target_lengths = target_lengths.to(device)
 
+            #print(inputs, targets) # works best with --batch-size 1
+
             input_lengths = encoder.subsampled_lengths(input_lengths)
 
             with torch.autocast(device_type='cuda', dtype=torch.float16):
                 outputs = encoder(inputs)
                 loss = recognizer(outputs, targets, input_lengths, target_lengths)
 
             if torch.isnan(loss):
@@ -112,15 +134,15 @@
                 print(f'[{epoch + 1}, {i + 1:5d}] time: {t1-t0:.3f} loss: {train_loss:.3f} grad_norm: {grad_norm:.3f}', flush=True)
                 wandb.log({'train/loss': train_loss, 'train/grad_norm': grad_norm})
                 t0 = t1
 
     @torch.inference_mode()
     def evaluate(self, epoch, valid_loader):
         device = self.args.device
-        encoder, recognizer, vocabulary = self.encoder, self.recognizer, self.vocabulary
+        encoder, recognizer, vocabulary = self.encoder, self.recognizer, self.vocab
 
         valid_loss = 0.
         lers = []
 
         encoder.eval()
         recognizer.eval()
         for i, (inputs, targets, input_lengths, target_lengths) in enumerate(valid_loader):
@@ -136,101 +158,122 @@
 
             valid_loss += loss.item()
 
             if i < 10:
                 outputs = recognizer.log_probs(outputs)
                 for ref, ref_len, seq, hyp_len in zip(targets, target_lengths, outputs, input_lengths):
                     seq = seq[:hyp_len].cpu()
+                    ref = ref[:ref_len].cpu().tolist()
                     #print('greedy', seq.argmax(dim=-1).tolist())
                     decoded = ctc_beam_search_decode_logits(seq)
                     hyp1 = vocabulary.decode(filter(None, decoded[0][0]))
-                    ref1 = vocabulary.decode(ref[:ref_len])
-                    hyp, ref = list(zip(*align(hyp1, ref1, '*')))
+                    ref1 = vocabulary.decode(ref)
 
                     dist = edit_distance(hyp1, ref1)
                     dist['length'] = len(ref1)
                     dist['ler'] = round(dist['total'] / dist['length'], 2)
+                    lers.append(dist['ler'])
 
-                    if i == 0:
-                        console.print('hyp', ' '.join(h.replace(' ', '_') for h in hyp), overflow='crop')
-                        console.print('ref', ' '.join(r.replace(' ', '_') for r in ref), overflow='crop')
-                        print(dist)
+                    if isinstance(ref1, str):
+                        star = '*'
+                        hyp, ref = list(zip(*align(hyp1, ref1, star)))
+
+                        if i == 0:
+                            console.print('hyp', ' '.join(h.replace(' ', '_') for h in hyp), overflow='crop')
+                            console.print('ref', ' '.join(r.replace(' ', '_') for r in ref), overflow='crop')
+                            print(dist)
+                    else:
+                        star = 42 # b'*'
+                        hyp, ref = list(zip(*align(hyp1, ref1, star)))
+                        hyp, ref = bytes(hyp), bytes(ref)
+
+                        if i == 0:
+                            console.print('hyp', hyp)
+                            console.print('ref', ref)
+                            print(dist)
 
-                    lers.append(dist['ler'])
 
         count = i + 1
         ler = round(sum(lers) / len(lers), 3)
         print(f'valid [{epoch + 1}, {i + 1:5d}] loss: {valid_loss / count:.3f} sample ler: {ler:.3f}', flush=True)
         if wandb.run is not None:
             wandb.log({'valid/loss': valid_loss / count, 'valid/ler': ler})
         return valid_loss / count
 
 
-def main():
+def make_parser():
     class Formatter(argparse.ArgumentDefaultsHelpFormatter,
                     argparse.MetavarTypeHelpFormatter):
         pass
 
     parser = argparse.ArgumentParser(formatter_class=Formatter)
     parser.add_argument('--init', type=Path, help="Path to checkpoint to initialize from")
     parser.add_argument('--save', type=Path, default='ckpt.pt', help="Path to save checkpoint to")
     parser.add_argument('--log-interval', type=int, default=100, help="Number of batches between printing training status")
     parser.add_argument('--num-epochs', type=int, default=30, help="Number of epochs to train for")
     parser.add_argument('--device', type=str, default='cuda:1', help="torch device to use")
     parser.add_argument('--batch-size', type=int, default=16, help="Batch size")
     parser.add_argument('--lr', type=float, default=3e-4, help="Adam learning rate")
     parser.add_argument('--train', type=str, help="Datasets to train on, comma separated")
     parser.add_argument('--eval', type=str, default='dev-clean', help="Datasets to evaluate on, comma separated")
-    parser.add_argument('--encoder', type=str, default='uni', choices=['uni', 'bi'], help="Encoder to use: unidirectional LSTM or bidirectional Transformer")
+    parser.add_argument('--encoder', type=str, default='lstm', choices=['lstm', 'r9'], help="Encoder to use: unidirectional LSTM or ResNet")
     parser.add_argument('--compile', action='store_true', help="torch.compile the model (produces incompatible checkpoints)")
     parser.add_argument('--star-penalty', type=float, default=None, help="Star penalty for Star CTC. If None, train with regular CTC")
     parser.add_argument('--num-workers', type=int, default=32, help="Number of workers for data loading")
     parser.add_argument('--glottal-closures', action='store_true', help="Add glotal closures to the vocabulary")
-    args = parser.parse_args()
+    parser.add_argument('--vocab', type=str, default='bytes', choices=['bytes', 'cmu', 'xen'], help="Vocabulary to use: raw bytes, CMUdict, Xen (CMUdict + glottal closures)")
+    return parser
+
 
+def main():
+    args = make_parser().parse_args()
     print(args)
 
     torch.manual_seed(3407)
 
     system = System(args)
 
     valid_loader = torch.utils.data.DataLoader(
         concat_datasets(args.eval),
-        collate_fn=Collator(system.vocabulary),
+        collate_fn=Collator(system.vocab),
         batch_size=16,
         shuffle=False,
         num_workers=args.num_workers,
     )
 
     if args.init:
         checkpoint = torch.load(args.init, map_location=args.device)
         system.load_state_dict(checkpoint)
+    else:
+        print('initializing randomly')
 
     if args.compile:
-        system = torch.compile(system, options={'trace.graph_diagram': True})
+        system = torch.compile(system, mode='reduce-overhead')
+
+    print('model parameters', sum(p.numel() for p in system.parameters() if p.requires_grad))
 
     if args.train:
         wandb.init(project='ha', config=args)
 
         train_loader = torch.utils.data.DataLoader(
             concat_datasets(args.train),
-            collate_fn=Collator(system.vocabulary),
+            collate_fn=Collator(system.vocab),
             batch_size=args.batch_size,
             shuffle=True,
             num_workers=args.num_workers,
             drop_last=True
         )
 
         best_valid_loss = float('inf')
         for epoch in range(args.num_epochs):
             system.train_one_epoch(epoch, train_loader)
 
             valid_loss = system.evaluate(epoch, valid_loader)
             if valid_loss < best_valid_loss:
                 best_valid_loss = valid_loss
                 print('saving model', args.save)
-                torch.save(system.state_dict(best_valid_loss=best_valid_loss, epoch=epoch), args.save)
+                torch.save(system.make_state_dict(best_valid_loss=best_valid_loss, epoch=epoch), args.save)
     else:
         system.evaluate(-100, valid_loader)
 
 if __name__ == '__main__':
     main()
```

### Comparing `haloop-0.0.5/ha/model.py` & `haloop-0.0.6/ha/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
             input_lengths = torch.full((features.shape[0],), features.shape[1], dtype=torch.long)
         if target_lengths is None:
             target_lengths = torch.full((features.shape[0],), len(targets), dtype=torch.long)
 
         with torch.autocast(device_type='cuda', dtype=torch.float32):
             logits = self.log_probs(features).to(torch.float32)
             logits = logits.permute(1, 0, 2) # T, N, C
-            #loss = self.ctc(logits, targets, input_lengths=input_lengths, target_lengths=target_lengths)
-            loss = ctc_reduce_mean(ctc_forward_score3(logits, targets, input_lengths, target_lengths), target_lengths)
+            loss = self.ctc(logits, targets, input_lengths=input_lengths, target_lengths=target_lengths)
+            #loss = ctc_reduce_mean(ctc_forward_score3(logits, targets, input_lengths, target_lengths), target_lengths)
             return loss
 
 
 class StarRecognizer(nn.Module):
     def __init__(self, feat_dim=1024, vocab_size=55+1, star_penalty=-1):
         super().__init__()
         self.classifier = nn.Linear(feat_dim, vocab_size)
```

### Comparing `haloop-0.0.5/ha/rnnlm.py` & `haloop-0.0.6/ha/rnnlm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from pathlib import Path
 import argparse
+import math
+from pathlib import Path
 
 from rich.console import Console
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import wandb
 
@@ -49,15 +50,15 @@
 
         output, state = self.rnn(emb, state)
         output = self.out_layer(output) # (T, N, V)
         output = output.transpose(0,1) # (N, T, V)
 
         return output, state
 
-    def init_hidden(self, batch_size):
+    def init_hidden(self, batch_size=1):
         weight = self.out_layer.weight
         h = weight.new_zeros(self.num_layers, batch_size, self.hidden_dim)
         c = weight.new_zeros(self.num_layers, batch_size, self.hidden_dim)
         return (h,c)
 
     def truncate_hidden(self, state):
         h,c = state
@@ -115,79 +116,84 @@
         self.scaler = torch.cuda.amp.GradScaler()
         if args.init:
             self.scaler.load_state_dict(checkpoint['scaler'])
 
         self.loss = nn.CrossEntropyLoss(ignore_index=0)
 
         self.log_interval = args.log_interval
-        if args.vocab_from_data:
-            self.prompts = args.complete
-        else:
-            self.prompts = [prompt.encode('utf-8') for prompt in args.complete]
         self.args = args
 
-    def state_dict(self):
+    def make_state_dict(self):
         return {
             'args': vars(self.args),
             'vocab': self.vocab.state_dict(),
             'model': self.model.state_dict(),
             'optimizer': self.optimizer.state_dict(),
             'scaler': self.scaler.state_dict(),
         }
 
     def prepare_prompt(self, prompt):
         device = next(self.model.parameters()).device
 
         prompt_list = [self.vocab.string_to_id[char] if isinstance(char, str) else char for char in prompt]
         x = torch.tensor(prompt_list).to(device).unsqueeze(1).long()
 
-        return x, self.model.init_hidden(1)
+        return x, self.model.init_hidden()
 
     @torch.inference_mode()
     def complete(self, prompt, steps=512, top_k=1):
         model = self.model
         model.eval()
 
-        joiner = ''
-        def cast(s):
-            nonlocal joiner
-            if isinstance(s, int):
-                joiner = b''
-                return s.to_bytes(1, 'big')
-            elif isinstance(s, bytes):
-                joiner = b''
-                return s
-            return s
-
-        out_list = []
         x, states = self.prepare_prompt(prompt)
 
+        # generate first token distribution, compute probability of the prompt
         logits, states = model(x, states)
-        prompt_logits = nn.functional.cross_entropy(logits[:-1], x[1:].view(-1), reduction='none').sum() / len(x[1:])
-
-        v, _ = torch.topk(logits, top_k)
-        logits[logits < v[:, [-1]]] = -float('Inf')
-        probs = F.softmax(logits, dim=-1)
-        probs = probs[-1]
-
-        ix = probs.multinomial(num_samples=1)
-
-        out_list.append(cast(self.vocab.id_to_string[int(ix)]))
-        x = ix.unsqueeze(1)
+        prompt_logits = nn.functional.cross_entropy(logits[:-1], x[1:].view(-1), reduction='none').sum()
+        prompt_logits_base2 = prompt_logits / math.log(2)
+        prompt_bits_per_token = prompt_logits_base2 / len(x[1:])
+
+        if steps > 0:
+            out_list = []
+            joiner = ''
+            def cast(s):
+                nonlocal joiner
+                if isinstance(s, int):
+                    joiner = b''
+                    return s.to_bytes(1, 'big')
+                elif isinstance(s, bytes):
+                    joiner = b''
+                    return s
+                return s
 
-        # decode
-        for k in range(steps):
-            logits, states = model(x, states)
+            # sample first token
             v, _ = torch.topk(logits, top_k)
             logits[logits < v[:, [-1]]] = -float('Inf')
             probs = F.softmax(logits, dim=-1)
+            probs = probs[-1]
+
             ix = probs.multinomial(num_samples=1)
+
+            # output first token only if we're asked to generate any samples
             out_list.append(cast(self.vocab.id_to_string[int(ix)]))
-            x = ix
-        return prompt_logits, joiner.join(out_list)
+            x = ix.unsqueeze(1)
+
+            # generate remaining tokens
+            for k in range(steps-1):
+                logits, states = model(x, states)
+                v, _ = torch.topk(logits, top_k)
+                logits[logits < v[:, [-1]]] = -float('Inf')
+                probs = F.softmax(logits, dim=-1)
+                ix = probs.multinomial(num_samples=1)
+                out_list.append(cast(self.vocab.id_to_string[int(ix)]))
+                x = ix
+
+            return prompt_bits_per_token, joiner.join(out_list)
+        else:
+            return prompt_bits_per_token, []
 
     def train_one_epoch(self, epoch=0, step=0):
         model, batches = self.model, self.batches
         optimizer, scaler, loss_fn = self.optimizer, self.scaler, self.loss
 
         state = model.init_hidden(self.args.batch_size)
         model.train()
@@ -224,15 +230,16 @@
 
             scaler.step(optimizer)
             scaler.update()
             optimizer.zero_grad(set_to_none=True)
 
             if i % self.log_interval == 0:
                 _, outputs = self.evaluate()
-                print(f"epoch {epoch} step {i}/{len(batches)} loss: {loss.item():.3f} ppl: {loss.exp().item():.3f} grad_norm: {grad_norm.item():.3f} {'; '.join(outputs)}")
+                train_bpc = loss.item() / math.log(2)
+                print(f"epoch {epoch} step {i}/{len(batches)} loss: {loss.item():.3f} ppl: {loss.exp().item():.3f} bpc: {train_bpc:.3f} grad_norm: {grad_norm.item():.3f} {'; '.join(outputs)}")
                 wandb.log({'train/loss': loss.item(),
                            'train/ppl': loss.exp().item(),
                            'train/lr': self.args.lr,
                            'train/epoch': epoch,
                            'train/grad_norm': grad_norm.item()})
                 model.train()
             else:
@@ -247,47 +254,72 @@
                 break
 
         return i+1
 
     def evaluate(self):
         prompt_scores = []
         outputs = []
-        for prompt in self.prompts:
+
+        def prompt_stream():
+            for prompt in (self.args.complete or []):
+                yield self.args.start_token + prompt
+            for prompt_file in (self.args.complete_file or []):
+                with open(prompt_file) as f:
+                    for line in f:
+                        utterance_id, text = line.strip().split(maxsplit=1)
+                        yield self.args.start_token + text
+
+        for prompt in prompt_stream():
+            if not self.args.vocab_from_data:
+                prompt = prompt.encode('utf-8')
             prompt_score, completion = self.complete(prompt, self.args.bptt_len, top_k=self.args.top_k)
-            if isinstance(completion, bytes):
-                outputs.append(str(prompt + completion, 'utf-8', errors='replace'))
+            output = prompt + completion if completion else prompt
+            if not self.args.vocab_from_data:
+                outputs.append(str(output, 'utf-8', errors='replace'))
             else:
-                outputs.append(prompt + completion)
+                outputs.append(output)
             prompt_scores.append(prompt_score.item())
-        return prompt_scores, outputs
+
+        return torch.tensor(prompt_scores), outputs
 
 
 def main():
     class Formatter(argparse.ArgumentDefaultsHelpFormatter,
-                    argparse.MetavarTypeHelpFormatter):
+                    argparse.MetavarTypeHelpFormatter,
+                    argparse.RawDescriptionHelpFormatter):
         pass
 
-    parser = argparse.ArgumentParser(description="hal trains recurrent language models", formatter_class=Formatter)
+    parser = argparse.ArgumentParser(description="hal trains recurrent language models",
+                                     formatter_class=Formatter, epilog="""\
+To produce 10-token completions of two strings try:
+% hal --init librispeech-1024.pt --rnn-size 1024 --bptt-len 10 --complete "IS THIS A BIRD" "IS THIS A PLANE"
+
+To compute BPC on evaluation data from files (first column is ignored) try:
+% hal --init librispeech-1024.pt --bptt-len 0 --rnn-size 1024 --complete-file LibriSpeech/dev-clean/*/*/*.txt
+
+␄
+""")
     parser.add_argument('--init', type=Path, help="Path to checkpoint to initialize from")
     parser.add_argument('--save', type=Path, default='rnnlm.pt', help="Path to save checkpoint to")
     parser.add_argument('--device', type=str, default='cuda:1', help='device')
     parser.add_argument('--lr', default=0.002, type=float, help='Adam learning rate')
     parser.add_argument('--dropout', default=0, type=float, help='dropout rate')
     parser.add_argument('--epochs', default=1, type=int, help='number of training set iterations')
     parser.add_argument('--max-steps', default=-1, type=int, help='maximum number of training steps per epoch (useful for e.g. lr search)')
     parser.add_argument('--batch-size', default=1280, type=int, help='batch size')
-    parser.add_argument('--bptt-len', default=256, type=int, help='RNN window size')
+    parser.add_argument('--bptt-len', default=256, type=int, help='RNN sequence length (window size)')
     parser.add_argument('--rnn-size', default=2048, type=int, help='RNN width')
     parser.add_argument('--num-layers', default=1, type=int, help='RNN depth')
     parser.add_argument('--vocab-from-data', action='store_true', help='build character vocabulary from the data')
     parser.add_argument('--train', type=Path, help='Train model on this data')
     parser.add_argument('--top-k', type=int, default=1, help='top-k sampling')
     parser.add_argument('--log-interval', type=int, default=100, help="Number of batches between printing training status")
-    #parser.add_argument('--complete, type=str, nargs='+', default=['\nа', '\nя'], help="Prompts to complete during evaluation")
-    parser.add_argument('--complete', type=str, nargs='+', default=['\nhello', '\nwhat '], help="Prompts to complete during evaluation")
+    parser.add_argument('--complete', type=str, nargs='+', help="Prompts to complete during evaluation")
+    parser.add_argument('--start-token', type=str, default='\n', help="Prepend this token to every prompt. This token is necessary to compute p(prompt|start-token)")
+    parser.add_argument('--complete-file', type=Path, nargs='+', help="Prompts to complete during evaluation as a file. First column is utterance id.")
     parser.add_argument('--num-workers', type=int, default=8, help="Number of workers for data loading")
     args = parser.parse_args()
 
     torch.manual_seed(3407)
 
     self = System(args)
 
@@ -295,17 +327,19 @@
         print(args)
         wandb.init(project='rnnlm', config=args)
 
         step = 0
         try:
             for epoch in range(args.epochs):
                 step = self.train_one_epoch(epoch=epoch, step=step)
-                torch.save(self.state_dict(), args.save)
+                torch.save(self.make_state_dict(), args.save)
         except KeyboardInterrupt:
             print('interrupted, saving')
-            torch.save(self.state_dict(), args.save)
+            torch.save(self.make_state_dict(), args.save)
 
-    for prompt_score, completion in zip(*self.evaluate()):
-        print('{:.2f}'.format(prompt_score), completion)
+    prompt_scores, outputs = self.evaluate()
+    for prompt_score, output in zip(prompt_scores, outputs):
+        print('{:.2f}'.format(prompt_score), 'bpc', output)
+    print('mean bpc', torch.mean(prompt_scores).item())
 
 if __name__ == '__main__':
     main()
```

### Comparing `haloop-0.0.5/ha/star.py` & `haloop-0.0.6/ha/star.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.5/ha/symbol_tape.py` & `haloop-0.0.6/ha/symbol_tape.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,27 +39,33 @@
 
     def add_new_word(self, string):
         self.string_to_id[string] = len(self.string_to_id)
         self.id_to_string[len(self.id_to_string)] = string
 
     # Given a string, return ID
     def get_idx(self, string, extend_vocab=False):
+        byte = bytes([ord(string)])
         if string in self.string_to_id:
             return self.string_to_id[string]
+        elif byte in self.string_to_id:
+            return self.string_to_id[byte]
         elif extend_vocab:  # add the new word
             self.add_new_word(string)
             return self.string_to_id[string]
         else:
             return self.unk_id
 
     def encode(self, text, extend_vocab=False):
         return torch.LongTensor([self.get_idx(char, extend_vocab=extend_vocab) for char in text])
 
     def decode(self, ids):
-        return ''.join([self.id_to_string[id] for id in ids])
+        if isinstance(self.id_to_string[0], bytes):
+            return b''.join([self.id_to_string[id] for id in ids])
+        else:
+            return ''.join([self.id_to_string[id] for id in ids])
 
     @classmethod
     def bytes(cls):
         self = Vocabulary(pad_token=0, unk_token=7)
         self.id_to_string = {}
         self.string_to_id = {}
```

### Comparing `haloop-0.0.5/ha/xen.py` & `haloop-0.0.6/ha/xen.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,23 @@
             }
             self.rdictionary.extend(["bcl", "tcl", "dcl", "gcl", "pcl", "kcl"])
         else:
             self.closures = {}
 
         self.dictionary = {c: i for i, c in enumerate(self.rdictionary, start=1)}
 
+    def state_dict(self):
+        return {
+            'rdictionary': self.rdictionary,
+        }
+
+    def load_state_dict(self, state_dict):
+        self.rdictionary = state_dict['rdictionary']
+        self.dictionary = {c: i for i, c in enumerate(self.rdictionary, start=1)}
+
     def __len__(self):
         return len(self.rdictionary) + 1
 
     def encode(self, text):
         labels = [phoneme.replace('2', '0')
                   for c in self.g2p(text)
                   if c != "'"
```

### Comparing `haloop-0.0.5/pyproject.toml` & `haloop-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "haloop"
 description = 'speech agent for 100 hours'
 readme = "README.md"
 requires-python = ">=3.9"
-license = "MIT"
+license = "GPL-3.0-or-later"
 keywords = []
 authors = [
   { name = "Volodymyr Kyrylov", email = "vol@wilab.org.ua" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
```

### Comparing `haloop-0.0.5/PKG-INFO` & `haloop-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: haloop
-Version: 0.0.5
+Version: 0.0.6
 Summary: speech agent for 100 hours
 Project-URL: Documentation, https://github.com/proger/ha1#readme
 Project-URL: Issues, https://github.com/proger/ha1/issues
 Project-URL: Source, https://github.com/proger/ha1
 Author-email: Volodymyr Kyrylov <vol@wilab.org.ua>
-License-Expression: MIT
+License-Expression: GPL-3.0-or-later
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
```

