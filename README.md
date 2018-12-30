A simple command line program to get Youtube channel RSS feed URL given a youtube video,
user, or channel link.

# Why

You can paste the output to your favorite feed reader application to subscribe to
Youtube channel without having an account. (Alternatively, you can use my other program,
[Vidlist](https://github.com/dxwc/vidlist#readme) that does both at the same
time and generates video thumbnails.)

# Install

1. Have [Node.js](https://nodejs.org/en/) installed
2. Run command **`npm install -g vidfeed@latest`** and you are all set
    + To update to latest version anytime after installation, run:
      `npm update -g vidfeed`
    + To uninstall, run: `npm uninstall -g vidfeed`
    + _Unix may need `sudo` before commands_
    + _Windows may need running cmd as administrator_

# Use

+ `vf <a copy pasted youtube video, user or channel url>` and press enter.
  Example:
    + `vf https://www.youtube.com/watch?v=ZiXZsMIVGos`
    + `vf https://www.youtube.com/user/PBSNewsHour`
+ If the copied link looks odd, it's a good idea to put it in quote to not upset your
  terminal emulator or command line prompt like. Example :
    + `vf "https://www.youtube.com/watch?time_continue=277&v=ZiXZsMIVGos"`
+ To view instruction or information, type and enter `vf --help`
+ **Note**: The program will run the same with the names: `vf`, `vidFeed` or `vidfeed`

# How

+ If channel ID can be found in input URL, does a string concatenation and prints
+ Else, downloads the page at input URL or something close to it and then looks though
  the downloaded page for channel ID information. Concatenate string and then print

---

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.