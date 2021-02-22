_**Nota bene:**_ This project is entirely unsupported.
I have not been able to get it to work, so creating an issue asking for guidance would be futile.
If you have files to contribute, or build instructions / documentation that others might find useful, awesome!
[Please submit a PR here](https://github.com/chbrown/candc/compare).

# candc

The canonical site, <http://svn.ask.it.usyd.edu.au/trac/candc>, is totally down.

Luckily, the Wayback Machine has archived most of that site:

* Latest capture of the [C&C tools main page](http://web.archive.org/web/20160318193242/http://svn.ask.it.usyd.edu.au/trac/candc)

Unfortunately, James Curran put all the downloads behind a registration wall, so the Wayback Machine doesn't have any records of those.

Fortunately, by the time I got around to creating this repository, Stephen Clark still hosted a copy of the downloads on his Cambridge website, <http://www.cl.cam.ac.uk/~sc609/candc-1.00.html> ([latest capture on the Wayback Machine](https://web.archive.org/web/20180727140643/http://www.cl.cam.ac.uk/~sc609/candc-1.00.html)).
The files available there were the 1.00 version, so not the latest version of everything, but better than nothing!

~That site and files are currently still live and accessible, but~ because I _knew_ that would happen, I downloaded and added them to this repository. The following section is taken verbatim from Stephen Clark's "C&C Parser Downloads" page.


## Version 1.0 9/06/07

* source code:
  <a href="downloads/candc-1.00.tgz">gzipped tar</a>

* precompiled binaries (do not contain Boxer):
  - Linux (static linked) <a href="downloads/candc-linux-1.00.tgz">gzipped tar</a> (12MB)
  - Mac OS X 10.4 (universal) <a href="downloads/candc-macosxu-1.00.tgz">gzipped tar</a> (12MB)

* models trained on CCGbank 02-21 and MUC 7:
  <a href="downloads/models-1.02.tgz">gzipped tar</a> (50MB)

* other models:
  - POS model trained on Penn Treebank 3:
    <a href="downloads/ptb_pos-1.00.tgz">gzipped tar</a> (6MB)
  - chunk model trained on Penn Treebank 3:
    <a href="downloads/ptb_chunk-1.00.tgz">gzipped tar</a> (4MB)
  - MUC 7 model (uses Penn Treebank 3 POS tags):
    <a href="downloads/ptb_muc-1.00.tgz">gzipped tar</a> (4MB)

* models for biomedical parsing
  - POS model (v1.00, 1/12/09):
    <a href="downloads/pos_bio-1.00.tgz">gzipped tar</a> (15MB)
  - supertagging model (v1.00, 1/12/09):
    <a href="downloads/super_bio-1.00.tgz">gzipped tar</a> (45MB)
  - markedup_sd file:
    <a href="downloads/markedup_sd-1.00">markedup_sd</a>
  - Post-processing script: grs2depbank (already current in parser 1.00) or grs2sd:
    <a href="downloads/grs2sd-1.00">grs2sd</a>


## License

I have no idea. Creative Commons should come up with something for abandonware.


## Other resurrections

An [Inria researcher](https://github.com/valeriobasile) runs a live demo server at <http://valeriobasile.github.io/candcapi/>

To repeat the needlessly heteronormative example from that page (_the patriarchy is strong with this one_):

    curl -d 'Every man loves a woman' 'http://gingerbeard.alwaysdata.net/candcapi/proxy.php/raw/pipeline?semantics=fol'

> fol(1,not(some(A,and(n1man(A),not(some(B,some(C,and(r1patient(B,C),and(r1agent(B,A),and(v1love(B),n1woman(C))))))))))).
