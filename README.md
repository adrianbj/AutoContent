AutoContent
================

ProcessWire module for automatic generation of content when a field is blank and also for generating test pages that can be "one-click" deleted.

Currently works for most default PW fieldtypes. Profields and selected third party fieldtypes coming shortly.

### Currently supported field types
Others may work, but these are the ones that have currently been tested. Support for Profields and others is coming soon.

#### Core
* Text
* Textarea (RTE and plain) - content generated from http://loripsum.net/ API
* Page
* Datetime
* Integer
* Float
* Email
* URL
* Image - images generated by http://placehold.it using the field's min and max settings

#### 3rd Party
* MapMarker

### CONFIG SETTINGS

#### Module settings
You can change the locale which affects the content generated by the Faker library in text fields.

#### Field settings
Config settings for certain field types are available from the field's Input tab under the AutoContent Options section.

##### Textarea
There are multiple options for determing the content of the generated lorem ipsum text.
* number of paragraphs to generate.
* short, medium, long, verylong - The average length of a paragraph.
* decorate - Add bold, italic and marked text.
* link - Add links.
* ul - Add unordered lists.
* ol - Add numbered lists.
* dl - Add description lists.
* bq - Add blockquotes.
* code - Add code samples.
* headers - Add headers.

If the textarea inputfield type is not an RTE, then only the first two are available and output with be plain text.

##### Text
Generated content attempts to make use of the include Faker (https://github.com/fzaninotto/Faker) library.
The name of the field will attempted to be matched to available Faker properties automatically.
If there is no match, you can manually provide one under the Faker property config setting.


### License

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.

(See included LICENSE file for full license text.)