# swift-guessing-game
guessing game using swift.  I have the first page set, but can't figure out how to code a reset for a new game 
with new text and new pic for each reset.  


import UIKit

class ViewController: UIViewController {
        

        var pushIn = 0 

        @IBOutlet weak var iResp: UILabel!
        
        @IBOutlet weak var justText: UITextField!
        
        @IBAction func submit(_ sender: Any) {
            // toggle my code
            
            pushIn = pushIn + 1
            
            if pushIn == 1 {
                iResp.text = "Nah, 2 more chances!"
            } else if pushIn == 2 {
                iResp.text = "Really? "
            } else {
                iResp.text = "WRONG! Click if you want to start over."            
            }
          
        }
        
        override func viewDidLoad() {
            super.viewDidLoad()
            iResp.text = “Can you figure it out?"
            
            //screen color
            view.backgroundColor = .yellow}
        
        override func didReceiveMemoryWarning() {
            super.didReceiveMemoryWarning()
            
        }

}
