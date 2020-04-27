# Tour Guide App

For this project, they asked to create a tourist guide application. It has been developed with support for screen rotation (Portait / Landscape) application with multiple screens, each of which lists a type of attraction.

Has :
1 RecyclerView, Adapter, Custom classes, All Strings, dimensions, theme of the app, must go separately. It is a requirement and in addition to good coding practices.
The images have been placed in their respective drawables directory in the corresponding folder for the support of different types of resolutions.

Note: It was not a requirement that links to another activity when you tap on the recyclerview images.


Your project will be evaluated using the Tour Guide App project rubric.
<div id="proj-spec-div" class="col-xs-offset-1 col-xs-10"> <h2 id="project-spec-headline" translate="" class="ng-scope">Project Specification</h2> <h3 id="project-name" ng-bind-html="localize(ctrl.rubric.project, 'name', markup=true)" class="ng-binding"><p>Tour Guide App</p>
</h3> <div rubric-table="" rubric="ctrl.rubric" settings="ctrl.tableSettings" class="ng-isolate-scope"><!-- ngRepeat: section in rubric.sections --><div ng-repeat="section in rubric.sections" class="ng-scope" style=""> <span class="rubric-section ng-binding" ng-bind-html="localize(section, 'name', markup=true)"><p>Layout</p>
</span> <table class="table table-bordered section-table"> <thead> <tr> <!-- ngIf: !rubric.hide_criteria --><th class="rubric-category criteria-column col-xs-3 ng-scope" ng-if="!rubric.hide_criteria"> <span translate="" class="ng-scope">Criteria</span> </th><!-- end ngIf: !rubric.hide_criteria --> <th class="rubric-category meets-specs-column" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)"> <span translate="" class="ng-scope">Meets Specifications</span> </th> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr> </thead> <tbody>  <!-- ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Overall Layout</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>App contains at least 4 lists of relevant attractions for a location</p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Navigation</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>User navigates between lists in Fragments using either a Navigation Drawer or a ViewPager plus TabLayout. </p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>List Item Contents</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>Each list item contains information about an event, restaurant, historical site, or similar. </p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Pictures</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>At least one list includes pictures of the location. </p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Layout Best Practices</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>The code adheres to all of the following best practices:</p>
<ul>
<li>Text sizes are defined in sp</li>
<li>Lengths are defined in dp</li>
<li>Padding and margin is used appropriately, such that the views are not crammed up against each other.</li>
</ul>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --> </tbody> </table> </div><!-- end ngRepeat: section in rubric.sections --><div ng-repeat="section in rubric.sections" class="ng-scope"> <span class="rubric-section ng-binding" ng-bind-html="localize(section, 'name', markup=true)"><p>Functionality</p>
</span> <table class="table table-bordered section-table"> <thead> <tr> <!-- ngIf: !rubric.hide_criteria --><th class="rubric-category criteria-column col-xs-3 ng-scope" ng-if="!rubric.hide_criteria"> <span translate="" class="ng-scope">Criteria</span> </th><!-- end ngIf: !rubric.hide_criteria --> <th class="rubric-category meets-specs-column" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)"> <span translate="" class="ng-scope">Meets Specifications</span> </th> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr> </thead> <tbody>  <!-- ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Location Object</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>App contains a custom object for storing location information .</p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Custom Adapter</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>App uses a custom adapter to populate the layout with views based on instances of the custom class. </p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>String Storage</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>All strings are stored in the strings.xml resource file.</p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Image Storage</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>All images are stored as drawables. </p>
<p>All drawables are stored at multiple densities. </p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Errors</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>The code runs without errors. </p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --> </tbody> </table> </div><!-- end ngRepeat: section in rubric.sections --><div ng-repeat="section in rubric.sections" class="ng-scope"> <span class="rubric-section ng-binding" ng-bind-html="localize(section, 'name', markup=true)"><p>Code Readability</p>
</span> <table class="table table-bordered section-table"> <thead> <tr> <!-- ngIf: !rubric.hide_criteria --><th class="rubric-category criteria-column col-xs-3 ng-scope" ng-if="!rubric.hide_criteria"> <span translate="" class="ng-scope">Criteria</span> </th><!-- end ngIf: !rubric.hide_criteria --> <th class="rubric-category meets-specs-column" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)"> <span translate="" class="ng-scope">Meets Specifications</span> </th> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr> </thead> <tbody>  <!-- ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Readability</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>Code is easily readable so that a fellow programmer can understand the purpose of the app.</p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Naming Conventions</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>All variables, methods, and resource IDs are descriptively named so that another developer reading the code can easily understand their function.</p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --><tr ng-repeat="rubricItem in section.rubric_items" class="ng-scope"> <!-- ngIf: !rubric.hide_criteria --><td class="rubric-item criteria col-xs-3 ng-binding ng-scope" ng-if="!rubric.hide_criteria" ng-bind-html="localize(rubricItem, 'criteria', markup=true)"><p>Formatting</p>
</td><!-- end ngIf: !rubric.hide_criteria --> <td class="rubric-item meets-spec ng-binding" ng-class="settings.showReviewerTips ? col-xs-4 : (settings.showCompletedChecklist ? col-xs-6 : col-xs-7)" ng-bind-html="localize(rubricItem, 'passed_description', markup=true)"><p>The code is properly formatted: </p>
<ul>
<li>No unnecessary blank lines</li>
<li>No unused variables or methods</li>
<li>No commented out code</li>
</ul>
<p>The code also has proper indentation when defining variables and methods.</p>
</td> <!-- ngIf: settings.showReviewerTips --> <!-- ngIf: settings.showCompletedChecklist --> </tr><!-- end ngRepeat: rubricItem in section.rubric_items --> </tbody> </table> </div><!-- end ngRepeat: section in rubric.sections --> </div> <!-- ngIf: ctrl.rubric.stand_out --> </div>

![image](https://github.com/androidtenerife/Tour-Guide-App/blob/master/tourguide.png)

