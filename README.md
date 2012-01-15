Doctrine2.tmbundle is a Textmate Bundle for writing lightning fast Doctrine 2 entities with annotations. It fully supports annotation format of Doctrine 2.2.

###Supported snippets and tab triggers :

Entity Template `template`

    <?php
    namespace Entities;

    /**
     * @Entity
     * @Table(name="table_name")
     */
    class EntityName
    {

        /**
         * @Id @Column(type="integer")
         * @GeneratedValue
         */
        private $id;
    
    
    }

Column `column`

    /**
     * @Column(type="string|integer|smallint|bigint|boolean|decimal|date|time|datetime|text|object|array|float", name="column_name", length=255, unique=false, nullable=false, precision=0, scale=0, columnDefinition="definition")
     */
    protected $field_name;
    

Id `ìd`

    /**
     * @Id @Column(type="integer")
     * @GeneratedValue
     */
    private $id;
    
Version `version`

    /**
     * @column(type="integer")
     * @version
     */
    protected $version;

Change Tracking Policy `changetracking`

    /**
     * @ChangeTrackingPolicy("DEFERRED_IMPLICIT|DEFERRED_EXPLICIT|NOTIFY")
     *
     */

Join Columns `joincol`

    /**
     * @JoinColumn(name="entity_id", referencedColumnName="id", unique=false, nullable=false, onDelete="cascade", columnDefinition="definition")
     *
     */

Join Table `jointable`

    /**
     * @JoinTable(name="table_name", joinColumns={}, inverseJoinColumns={}) 
     *
     */

Discriminator Column `discrcol`

    /**
     * @DiscriminatorColumn(name="column_name", type="column_type", length=255) 
     *
     */

Many To Many `manytomany`

    /**
     * @ManyToMany(targetEntity="EntityName", inversedBy="inverse_side", mappedBy="property_name", cascade="cascade_option", fetch="LAZY|EXTRA_LAZY|EAGER", indexBy="field_name") 
     *
     */

Discriminator Map `discrmap`

    /**
     * @DiscriminatorMap({"value" = "Class"}) 
     *
     */

Many To One `manytoone`

    /**
     * @ManyToOne(targetEntity="EntityName", cascade={"cascade_option"}, fetch="EAGER|LAZY", inversedBy="inverse_side")
     *
     */

Mapped Superclass `super`

    /**
     * @MappedSuperclass(repositoryClass="Namespace\Repository") 
     *
     */

Entity `entity`

    /**
     * @Entity(repositoryClass="Namespace\Repository", readOnly=false)
     *
     */

One To Many `onetomany`

    /**
     * @OneToMany(targetEntity="EntityName", cascade={"cascade_option"}, fetch="LAZY|EXTRA_LAZY|EAGER", mappedBy="entity", orphanRemoval=false, indexBy="field") 
     *
     */

Generated Value `generated`

    /**
     * @generatedValue(strategy="AUTO|SEQUENCE|IDENTITY|TABLE|NONE") 
     *
     */
  
One To One `onetoone`

    /**
     * @OneToOne(targetEntity="EntityName", cascade={"cascade_option"}, fetch="EAGER|LAZY", inversedBy="inverse_side", orphanRemoval=false) 
     *
     */

Has Lifecycle Callbacks `hascallbacks`

    /**
     * @HasLifecycleCallbacks 
     *
     */

Order By `orderby`

    /**
     * @OrderBy({"field" = "ASC|DESC"})
     *
     */

Sequence Generator `sequence`

    /**
     * @SequenceGenerator(sequenceName="tablename_seq", initialValue=1, allocationSize=100)
     *
     */

Index `index`

    /**
     * indexes={@index(name="index_name", columns={"column_name"})} 
     *
     */

Table `table`

    /**
     * @Table(name="table_name", uniqueConstraints={}, indexes={})
     *
     */

Inheritance Type `inheritance`

    /**
     * @InheritanceType("SINGLE_TABLE|JOINED")
     *
     */

Unique Constraint `unique`

    /**
     * @UniqueConstraint(name="index_name", columns={"column_name"})
     *
     */

Join Column `joincol`

    /**
     * @JoinColumn(name="entity_id", referencedColumnName="id", unique=false, nullable=false, onDelete="cascade", columnDefinition="definition")
     *
     */