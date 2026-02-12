# Secure Cut-Copy-Paste

Demonstrates use of BlackBerry Dynamics secure user interface text controls.

## Descriptions

The secure user interface text controls are compared with the corresponding default native Android controls:

-   AutoCompleteTextView
-   EditText
-   SearchView
-   TextView
-   WebView

Text in a BlackBerry Dynamics control may be encrypted before being written to the clipboard, and decrypted when read from the clipboard.

Secure controls can be created in 3 ways; each would guarantee the same security, they differ only with regards to the underlaying layout class.

-   Explicit use of Dynamics classes that subclass the standard Android controls: in layout xml use classes like com.good.gd.widget.GDTextView (it extends  android.widget.TextView) 
-   Explicit use of Dynamics classes that subclass the AppCompat Android controls: in layout xml use classes like com.good.gd.widget.GDAppCompatTextView (it extends androidx.appcompat.widget.AppCompatTextView)
-   Implicit use of Dynamics classes that subclass the AppCompat Android controls: in layout xml use classes like TextView which will be inflated as a GDAppCompatTextView by the Dynamics SDK


## Requirements

See [Software Requirements](https://docs.blackberry.com/en/development-tools/blackberry-dynamics-sdk-android/current/blackberry-dynamics-sdk-android-devguide/gwj1489687014271) of the BlackBerry Dynamics SDK (Android) 

## How To Build and Deploy

1. Set up BlackBerry Dynamics Development Environment.
2. Clone the repo. 
3. Launch Android Studio and open the project.
4. Edit the *GDApplicationID* to your own or use the default '*com.blackberry.dynamics.sample*' in the *settings.json* file in the assets directory .
5. Assign the app entitlement to a user in your UEM server. This may also require adding the BlackBerry Dynamics App entitlement to UEM if you are using your own. See [Add an internal BlackBerry Dynamics app entitlement](https://docs.blackberry.com/en/endpoint-management/blackberry-uem/current/managing-apps/managing-blackberry-dynamics-apps).
6. Build and run on emulator or a device.

For more information on how to develop BlackBerry Dynamics apps, refer to [Get Started with BlackBerry Dynamics](https://developers.blackberry.com/us/en/resources/get-started/blackberry-dynamics-getting-started) 

## License

Apache 2.0 License

## Disclaimer

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
