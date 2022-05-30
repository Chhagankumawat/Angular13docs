# Angular13docs

String Interpolation 
>> String interpolation is binding of a data inside curely bases.
ex.
<p>{{allowNewUser}}</p>

--------------------------------------------------------------------------------------------------
# (ngSwitch) in angular 
$(html file)
<select (change)="xyz($event)">
        <option value="">Select anyone</option>
        <option value="html">H</option>
        <option value="css">C</option>
        <option value="bootstrap">B</option>
        <option value="javascript">J</option>
        <option value="other">O</option>
    </select>
    <div [ngSwitch]="switch">
        <p *ngSwitchCase="'html'">HTML</p>
        <p *ngSwitchCase="'css'">CSS</p>
        <p *ngSwitchCase="'bootstrap'"> BOOTSTRAP</p>
        <p *ngSwitchCase="'javascript'">JAVASCRIPT</p>
        <p *ngSwitchDefault="'other'">PLEASE SELECT VALID</p>
    </div>
    
   $(ts file)
    switch=""
    xyz(abc:any){
        this.switch=abc.target.value;
    }
