# Fork

This is my personal fork of https://code.google.com/p/amphetype/

### Differences include:

1. Unicode -> Ascii transliteration to avoid "untypable characters", as well as some replacements of bad formatting, either via unidecode and/or manually (see Text.py)

2. Letter coloring, both in input and displayed text, based on current positions and errors

3. Invisible Mode: Makes input text invisible (for use with #2)

4. Toggle case sensitivity

5. Option for continuing to the next passage even with typing mistakes

4. Option for automatically inserting space, newline, and other custom letters

6. Option for preventing continuing to the next word until space correctly pressed

7. Extensive GUI Color Settings

8. Can change return and space characters

9. Allows for smaller resizing than vanilla Amphetype

### Todo:

1. Refactor so that data analysis is separate from GUI classes

2. Multiplayer?!

### Warning about databases/statistics: 

The database/statistics of this fork should be considered unstable.  In addition, some of the options here (e.g. automatically inserting spaces or other characters) can significantly change the resulting statistics. 

It is therefore recommended to use a different database for this fork than with other versions of amphetype, as well as to make regular backups of any important data.

# Screenshots

### Typer
![Typer](screenshots/typer.png)

# License and Disclaimers

Amphetype is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

Amphetype is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Amphetype.  If not, see <http://www.gnu.org/licenses/>.

THIS SOFTWARE, ANY ASSOCIATED FILES, AND ANY ASSOCIATED DOCUMENTATION
ARE PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS", WITHOUT
WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS
BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, ANY ASSOCIATED FILES,
OR ANY ASSOCIATED DOCUMENTATION, EVEN IF ADVISED OF THE POSSIBILITY OF
SUCH DAMAGE.

# Original

Proper install is coming. I apologize for the current
mess. It was developed on a Windows machine with few
tools and no internet during a train ride and suffered
a few rewrites so the filenames aren't very descriptive
anymore.


To run, type:

python Amphetype.py


Depends on:

python-qt4  (that is, PyQt 4.3+)

OPTIONAL:

unidecode from https://pypi.python.org/pypi/Unidecode/
 - Will attempt to transliterate unicode -> ascii using this,
 if available. The default methods are mostly manual 
 (see: unicode_replacements in Text.py) and probably not as 
 effective.

py-editdist from http://www.mindrot.org/projects/py-editdist/
 - This latter dependancy is by no means critical and you will
 probably never get to use it. (For fetching words from a wordfile
 that are "similar" to your target words in the lesson generator.)
 If you don't have the module it will just select random words
 instead



