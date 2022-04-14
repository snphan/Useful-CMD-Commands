# Useful CMD Commands

A list of useful CMD Commands that you can use on windows for file management and such. If you ever get stuck just do "help [Command]" without the quotations. 


## Basic Commands
Note that if your paths have spaces in them you need to encapsulate it with ONLY " ". For example if you have a path like New Folder 1/New Folder 2, you will need to input it as "New Folder 1/New Folder 2", or else CMD will treat the spaces as separate commands.
  <table>
    <tr>
      <th>Command</th>
      <th>Usage</th>
    </tr>
    <tr>
      <td>del [file_path]</td>
      <td>Delete a file</td>
    </tr>
    <tr>
      <td>copy [file_path] [copy to folder path]</td>
      <td>Copy a file to some folder</td>
    </tr>
    <tr>
      <td>del [file_path]</td>
      <td>Delete a file</td>
    </tr>
    <tr>
      <td>move [file_path] [move to folder path]</td>
      <td>move a file to some folder</td>
    </tr>
    <tr>
      <td>ren [old_filename] [new_filename]</td>
      <td>move a file to some folder</td>
    </tr>   
    <tr>
      <td>mkdir [folder_name]</td>
      <td>Make a new dir called "folder_name" in the current directory</td>
    </tr>   
    <tr>
      <td>cd [folder_path]</td>
      <td>Change working directory to folder_path</td>
    </tr>
  </table>

## Viewing Folder Commands
  <table>
    <tr>
      <th>Command</th>
      <th>Usage</th>
    </tr>
    <tr>
      <td>tree</td>
      <td>Shows a tree of the folder and its subdirectories</td>
    </tr>
    <tr>
      <td>dir</td>
      <td>Shows the files and folders</td>
    </tr>
    <tr>
      <td>dir /b /a-d</td>
      <td>List all of the files in the current directory</td>
    </tr>
  </table>


## Useful For Loops
Note that the %[letter] can be any letter. It just represents a variable in the CMD.
  <table>
    <tr>
      <th>Command</th>
      <th>Usage</th>
    </tr>
    <tr>
      <td>FOR /L %I in (0,1,10) DO mkdir "Folder %I"</td>
      <td>Make a bunch of incrementing folders called "Folder #" in the current directory. /L allows you to do ranges(start, step, end)</td>
    </tr>
    <tr>
      <td>FOR /L %I in (0,1,10) DO echo "FILE %I" > "File %I.txt"</td>
      <td>Create an incrementing list of text files and Write FILE # into each file.</td>
    </tr>
    <tr>
      <td>FOR /D %d in (*) DO mkdir "%d/New Folder"</td>
      <td>Make "New Folder" in all folders of current directory. You can change the (*) to some other format to select only specific files. For example (iot-*) folders that start with "iot-". You need the /D to loop through the folders</td>
    </tr>
    <tr>
      <td>FOR %a in (*.pdf) DO ren "%a" "0%a"</td>
      <td>Add a leading 0 to all of the files in the folder with .pdf extension</td>
    </tr>
    <tr>
      <td>FOR %a in (*.txt) DO ren "%~a" "%~na version 1%~xa"</td>
      <td>Add "version 1" right before .txt</td>
    </tr>
    <tr>
      <td>FOR /D %a in (*) DO FOR %b in ("%a/*.csv") DO copy "%a\%b" "..\New folder"</td>
      <td>Copy all .csvs from child directories to "New Folder" in the parent directory</td>
    </tr>
  </table>
dasdfasdfa
