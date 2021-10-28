# Useful CMD Commands

A list of useful CMD Commands that you can use on windows for file management and such. If you ever get stuck just do "help <Command>" without the quotations. 


## Basic Commands
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
  </table>


## Useful For Loops
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
      <td>FOR /D %d in (*) DO mkdir "%d/New Folder"</td>
      <td>Make "New Folder" in all folders of current directory. You can change the (*) to some other format to select only specific files. For example (iot-*) folders that start with "iot-"</td>
    </tr>
  </table>
