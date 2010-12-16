# Launch Deamons

These are a collection of daemons that I use to start services on my development machine. 

When developing I hate having to start and stop dependancies so I can work so instead I just 
let these guys take the pain away for me.

They should be placed in `/Library/LaunchDaemons` I have them `chown`'d to `root:wheel` I am 
not sure if that is important or not. You will need to update the files to use your own home 
folder.

You can manually add them to the lanuchd by calling 
`sudo launchctl load uk.co.e26.[...].plist`. They should start as soon as they are added to 
the daemon. If for what ever reason they have failed to start you can kick them by using 
`sudo launchctl start uk.co.e26.[...]` and stop with the appropriately named 
`sudo launchctl stop uk.co.e26.[...]`.


# Licence

Copyright (c) 2010 Edd Sowden

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
